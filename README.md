`a3-gitname-firstname-lastname`.

Sample Readme (delete the above when you're ready to submit, and modify the below so with your links and descriptions)
---

## Ken's Ice Cream Shop (Ver. 2)

http://a3-kendesrosiers.glitch.me

For this project, I built on what I did for project 2 and made my game a whol lot better and more user friendly. Most notibly, I got rid of the wonky drag/drop functionality and replaced it with registering different key presses associated with different flavors. This makes the game a lot easier to play. I faced a lot of challanges with getting the local authentication to work. For my app, I feel like the logging in functionality is kind of pointless, and I wouldn't have made a game if I knew we were going to implement a user authentication system. I did however really like the idea of persistent data storage. I went with the recommended lowdb, and I used it in order to have a persistant scoreboard. I used authentication to allow an admin to modify and delete entries from the scoreboard. Also, I ended up going with JWT (JSON Web Token) based authentication. For the quick login to change the scoreboard, I feel like the local strategy/storing cookies and creating sessions was a bit too complicated, so a token-based authentication worked just fine. I also had a bit of a hard time understanding the session/cookie idea. I used nes.css as my CSS framework because I already had the 8-bit styling last time. This framework helped me convert more things to 8-bit styling, like buttons and modals. For Express middleware, I used passport, passport-jwt, body-parser, serve-static, and serve-favicon. passport and passport-jwt were for authenticating the token that I generated with a different module (jsonwebtoken). body-parser was for easy json request/response parsing. serve-static was to help serve whole directories, and serve-favicon was to include a favicon on the tab of the game.

## Technical Achievements
- **jsonwebtoken**: I used this module in order to take a payload and create a jwt out of it for authentication.
- **Tech Achievement 2**: I changed the entire functionality of my game from drag/drop to key presses using javascript events.

### Design/Evaluation Achievements
- **level of difficulty**: I used nes.css radio buttons and a modal in order to allow the user to select what level of difficulty they want to play the game at.
