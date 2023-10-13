In this file, provide a detailed outline of how to use and user test your new feature(s)

Added “Be Right Back” status to user dropdown
1) Sign into NodeBB
2) Click on user icon in the upper right corner of page
3) Confirm that the “Be right back” status option is there with a blue dot to its left
4) Change your status to be “Be right back”
5) Click user icon again
6) Note how the circle next to your username (e.g. admin) is light blue
7) Click user icon again -> navigate to Settings in the dropdown menu
8) Change language of NodeBB, save changes
9) Note how “Be right back” changes language with the other status options 
10) Added testing with this PR: https://github.com/CMU-313/fall23-nodebb-michaels-angels/pull/28
<img width="154" alt="Screenshot 2023-10-12 at 8 33 09 PM" src="https://github.com/CMU-313/fall23-nodebb-michaels-angels/assets/124110177/282fb987-cdc6-4d08-a71e-77debc2b7b35">


Added “Endorse Reply” button on posts
1) Sign into NodeBB as an admin
2) Navigate to the General Discussion page
3) Make a post
4) Notice how the option “endorse reply” is present next to the “reply” and “quote” options on the bottom right of the post
5) When you click the “endorse reply” button there should be a green popup that reads “endorsed by [user that posted]” – note that the “endorsed by ___” name is the user who made the post, not your username, which is a bug we didn’t have time to fix (also no matter which “endorsed by” post you click, the “endorsed by ___” button appears on the 
<img width="553" alt="Screenshot 2023-10-12 at 8 34 47 PM" src="https://github.com/CMU-313/fall23-nodebb-michaels-angels/assets/124110177/e29bc2b9-fbe2-4939-9db7-82b9c1074707">


Added “Point System” for users
1) Clone our repo
2) Run ‘npm i @nodebb/nodebb-plugin-user-level@1.0.4’ in your terminal
3) Sign into NodeBB as an admin
4) Navigate to “admin” in your header bar
5) Click Extend → Plugins in your header bar
6) Search for nodebb/nodebb-plugin-user-level
7) Click on “Activate”
8) Rebuild and restart forum
9) Click on Plugins → User level in the admin control panel again
10) Create your own self-defined user levels [sample picture below]
<img width="563" alt="Screenshot 2023-10-12 at 8 35 53 PM" src="https://github.com/CMU-313/fall23-nodebb-michaels-angels/assets/124110177/1c9fa00c-c745-40e2-874b-adcaef72500a">
11) Go to an existing post on your NodeBB homescreen
12) You should now see a user level next to each user’s username when they post [pictured below]
<img width="566" alt="Screenshot 2023-10-12 at 8 36 40 PM" src="https://github.com/CMU-313/fall23-nodebb-michaels-angels/assets/124110177/17ec9cc4-6637-4f2f-91d7-81085fde1a2b">


Added “Q&A” for users
1) Clone our repo
2) Run ‘npm install nodebb-plugin-question-and-answer’ in the terminal
3) Go to admin control panel 
4) Go to extend —> plugins
5) Search for nodebb-plugin-question-and-answer
6) Click on activate
7) Rebuild and restart forum
8) Go to an existing topic and click on the gear icon
9) You should see an option to convert to a question and if a question has been posed, an option to mark a question as solved
<img width="565" alt="Screenshot 2023-10-12 at 8 37 19 PM" src="https://github.com/CMU-313/fall23-nodebb-michaels-angels/assets/124110177/a3f81012-f206-4e9e-bf6a-30b31b87eb23">

Testing custom hooks 
1) Run ./nodebb dev in terminal
2) Log of all newly registered hooks will show up
3) Interacting with nodebb will show when each hook is fired
   
![IMG_4416](https://github.com/CMU-313/fall23-nodebb-michaels-angels/assets/124110177/e143d205-5cb4-4e7f-bac8-7d0a24176bb0)
![IMG_7166](https://github.com/CMU-313/fall23-nodebb-michaels-angels/assets/124110177/4cb18ef3-db09-4786-9af1-2c73a76ae789)


