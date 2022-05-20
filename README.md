# go
Задание для курса Введение в Go


/* Client scripts module */
// declare const alert: any
declare const console: any

async function onInit(): Promise<void> {
    let numString = '';
    for (let i = 1; i < 101; i++) {
        if (i % 15 === 0) {
            numString += (i === 100 ? 'FizzBuzz' : ('FizzBuzz' + '\n'));
        } else if (i % 3 === 0) {
            numString += (i === 100 ? 'Fizz' : ('Fizz' + '\n'));
        } else if (i % 5 === 0) {
            numString += (i === 100 ? 'Buzz' : ('Buzz' + '\n'));
        } else {
            numString += (i === 100 ? i.toString() : (i.toString() + '\n'));
        }
    }
    // alert(numString);          // целиком не помещается 
    console.log(numString);
}
