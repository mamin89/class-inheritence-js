# class-inheritence-js

//static method 
class Governer {

    constructor(name, title, authority) {
          this.name = name;
          this.title = title;
          this.authority = authority;


    }
}


   
var governer = new Governer('Mina Amin', 'Governer', 'Sign')
console.log(governer);


//inheritence
class Person{

    constructor(name, job, hobbies) {
          this.name = name;
          this.job = job;
          this.hobbies = hobbies


    }
}
class PostalWorker extends Person {
    constructor(name, job, hobbies, experience, gender) {

    super(name, job, hobbies)

        this.experience= experience;
        this.gender = gender;
}

}


   
var person = new Person('nia', 'doctor', 'sleep');
var person2 = new PostalWorker('Juan', 'PostalWorker', 'sleep', '5 years', 'male');

console.log(person);
console.log(person2);


class Chef extends Person {
    constructor(name, job, hobbies, experience, gender) {

    super(name, job, hobbies)

        this.experience= experience;
        this.gender = gender;
}

}


   
var person = new Person('nia', 'doctor', 'sleep');
var person2 = new PostalWorker('Juan', 'PostalWorker', 'sleep', '5 years', 'male');
var person3 = new Chef('Jane', 'Chef', 'sleep', '10 years', 'female');
console.log(person);
console.log(person2);
console.log(person3);
