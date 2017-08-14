# Script roadmap

1. Ensures the ask_shell exists in the system.
1. Asks the project name.
1. Asks the place to record the backup file.
1. Asks the credentials informations, trigging the **asking_credentials** function.
    1. The ssh user are not allowed to be null.
    1. The server are not allowed to be null.
    1. The password are not allowed to be null. Hides the caracters when typing.
    1. The server path are not allowed to be null.
        1. Validates the answer.
            1. Forces user to writes the **absolute path** from server. Don't allow type something that does not starts with forward slash.
            1. Checks if there's multiples backslashes together.
        1. If the answer is not valid, asks again.
    1. Asks for port. This can be optional.
1. Do a quick check if the credentials are valid.
    1. If not valid, starts again the credentials asking with **asking_credentials**.
1. Confirms the informations, exposing all the informations inputed, excepts the password.
1. Then, trigger the **do_everything** function to perform the backup.