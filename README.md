# Password-Generator

A simple password generator that creates passwords of any length and saves them in an Excel file with the associated applications.

This password generator uses a total of 82 characters to create a password. If we assume that the fastest computer is capable of generating 2,147,483,600 keys per second, then a 10 digit password would take 203 years to guess.

             combinations = 82^10
            
                          = 13.744.803.133.596.058.624 / 2.147.483.600 Keys/sec
             
                          = 6.400.422.864 seconds
             
                          = 106.673.714,4 minutes
             
                          = 1.777.895,2 hours
                          
                          = 74.079 days
                          
                          = 203 years
                          
Here you can see an overview of the security of different password lengths:


| password length | number of combinations  | x minutes      | x hours       | x days    | x years   |
|-----------------|-------------------------|----------------|---------------|-----------|-----------|
| 5               | 3707398432              | 0,028          |               |           |           |
| 6               | 304006671424            | 2,4            |               |           |           |
| 7               | 24928547056768          | 193,5          | 3,2           |           |           |
| 8               | 2044140858654976        | 15864,6        | 264,4         | 11        |           |
| 9               | 167619550409708032      | 1300899        | 21681,6       | 903,4     | 2,5       |
| 10              | 13744803133596058624    | 106673714,4    | 1777895,2     | 74079     | 203       |
| 11              | 1127073856954876807168  | 8747244580,9   | 145787409,7   | 6074475,4 | 16642,4   |
| 12              | 92420056270299898187776 | 717274055630,4 | 11954567593,8 | 498106983 | 1364676,7 |




## Start Program

```bash
python main.py
```

Now you will be asked for the application the password is for. Then the length of the password is asked. A password will now be generated and displayed. It can be decided whether this password should be used or another should be generated.

```bash
Application:
Length:
>Here ist the generated password shown<
You want to keep this password (y/n):
```

If a password has been created, which is also used, this application password pair is stored in an Excel spreadsheet.

Because the passwords can be very cryptic, they are stored in the Excel spreadsheet to have an easy overview and the user does not forget them. It is a good idea to use the read-only option for the Excel spreadsheet so that you don't accidentally change anything.

The Excel spreadsheet looks like this:

| Applications | Passwords    |
|--------------|-------------|
| Facebook     | password123 |

Each time the code is running, the new entry is appended to the existing excel tabbel.



- last Update: 05.02.2022 - DD.MM.YYYY
