
------
## **Natalia Grischenok**
#### Junior Frontend Developer
#### Contact information:
#### Phone: +7 960 9916111
#### E-mail: last_dreams@bk.ru
------
### Briefly About Myself:
> I am new to Frontend Developer. Before these courses, I tried to study on my own using videos and materials on the Internet, but I realized that I needed to structure my training. 2 months ago I graduated from courses in Innopolis University on Frontend Developert.I hope I can learn to understand JS better here, learn how to ask questions correctly and find answers to them. But most importantly, I hope that I will learn to quickly complete all the tasks .
-------
###Skills and Proficiency:
* HTML5
* CSS/SASS/SCSS
* JavaScript Basics
* Git, GitHub Git Lab
* VS Code
* React Basics
-------
### Education
* courses "Frontend Developer" in Innopolis University
-------
### **Code example:**
#### Игра "Угадай число"
    const Game = () => {
        let Random = Math.floor(Math.random() * 10) + 1;
        let attempt = 5;

        const BotGame = (attempt) => {
            let NumRansom = Random;
            let User = prompt(`Угадай число от 1 до 10`);

            const FuncGame = () => {
                if (attempt == 1){
                    let End = confirm (`Попытки закончились, хотите сыграть еще?`);
                    if (End == true) {
                        Game();
                    } else { // конец игры при нажатии "отмена"
                        alert(`Игра закончена!`);
                        console.log (User);
                        console.log (NumRansom);
                        return;
                    }       
                }
                if (User === null){
                    alert(`Игра закончена!`);
                    console.log (NumRansom);
                    return;
                }

                User = parseInt(User);
            
                if  (User < NumRansom ) {
                    attempt--;
                    alert(`Не угадали! Загаданное число больше, осталось ${attempt} попыток!`);
                    console.log (NumRansom);
                    BotGame(attempt);
                } else if (User === NumRansom ) {
                    let Victory = confirm (`Поздравляю, Вы угадали!!!Загаданное число $    {NumRansom}!!!Хотели бы сыграть еще?`);
                    if (Victory == true) {
                        Game();
                    } else { // конец игры при нажатии "отмена"
                        alert(`Игра закончена!`);
                        console.log (User);
                        console.log (NumRansom);
                        return;
                    }
                } else if ( User > NumRansom ) {
                    attempt--;
                    alert(`Не угадали! Загаданное число меньше, осталось ${attempt} попыток!`);
                    console.log (NumRansom);
                    BotGame(attempt);
                } else { // при поптыке ввести любые символы "длрлорплопроп"
                    alert(`Введите число!`);
                    BotGame(attempt);
                }
            }
            FuncGame();
            return;
        }
        BotGame(5);
        return;
    }
    Game();
-----------
### **English**
* A2 