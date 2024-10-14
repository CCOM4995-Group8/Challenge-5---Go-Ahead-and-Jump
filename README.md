Firstly, we started with the basics. Simply add a Plane to act as a terrain for our character, and place the character in the terrain.

![{1E1CA309-BE92-42E0-84BE-E5BFD6157D9A}](https://github.com/user-attachments/assets/2c2c6e92-e9b5-41fe-bf3c-e91221db42c6)

Then, we add a new script called PlayerMovement. In this script, we will be using the old Input System.
To change the Input System version, go to Edit>Project Settings>Player>Other Settings, then change the
version to your preferred version:

![{0DA8C0F7-27D1-4360-8713-AB69022320AA}](https://github.com/user-attachments/assets/4cc9758a-d35f-4306-9008-1387d5ec23de)

Script variables:

![{3960FEC7-8C95-41E5-80F1-7D6D8A65E9E9}](https://github.com/user-attachments/assets/3be8b2f1-ac28-4dd0-bba6-0958f5273e71)

Script Body:

![{9761E8CB-8AE9-437E-996B-C3945B231751}](https://github.com/user-attachments/assets/9f3b0f3f-0c9c-44c7-a70d-3e912f5bebef)

With the following code lines, we were able to make the character run when the user presses Left Shift,
and we were able to make the character jump when the user presses Space.

 if (Input.GetKey(KeyCode.LeftShift))
        {
            transform.Translate(0, 0, speed*Time.deltaTime*2);
        }
        if (Input.GetKey(KeyCode.Space))
        {
            transform.Translate(0, speed*Time.deltaTime, 0);
        }

Results:

https://github.com/user-attachments/assets/489a040a-c8e9-494f-86ec-b3652f2d8936

