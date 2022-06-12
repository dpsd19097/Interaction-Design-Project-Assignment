# Lesson: Interaction Design

### First and Last Name: 
      Maria Stampoulou 
      Papari Evangelia
### University Registration Number: 
      dpsd19121 
      dpsd19097
### GitHub Personal Profile: 
      https://github.com/mar-stamp 
      https://github.com/dpsd19097

# Introduction

# Summary


# 1st Deliverable
	Brief: Ο σκοπός του project μας είναι ο προγραμματισμός κινούμενου ρομπότ με τη χρήση arduino uno το οποίο θα καθοδηγεί τους τυφλούς. Ο έλεγχος της κίνησης θα πραγματοποιείται από ηχητικούς αισθητήρες για την αποφυγή εμποδίων στον εξωτερικό χώρο. Το προϊόν θα συνδέεται μέσω κονταριού με τον καρπό του χρήστη.  
	Target group: Το υπό σχεδίαση προϊόν απευθύνεται στους τυφλούς, ηλικίας από 10-55 ετών. Οι χρήστες μας είναι ανεξαρτήτου φύλου.
	Πλαίσιο χρήσης: Οι χρήστες έχουν τη δυνατότητα να χρησιμοποιήσουν το προϊόν σε πλατείες, πάρκα, δρόμους, πεζοδρόμια, παιδικές χαρές και κήπους.
	Υλικά και εργαλεία: Arduino unο
                    Wires
                    LED lights/Αντιστάτες
                    Αισθητήρας υπερήχων (+ βάση)
                    Battery
		     Κοντάρι/ χερούλι καρπού
                    Motor driver
                    Breadboard
                    Robot smart car
                    Κατσαβίδι
                    Κόλλα
                    Σελοτέιπ/Μονωτική ταινία
                    Ψαλίδι
	Ανταγωνισμός: Εκπαιδευμένα σκυλιά-οδηγοί
	              Πλάκες πεζοδρομίων για τυφλούς (κίτρινα)
		      Μπαστούνι στήρηξης για τυφλούς
		    
# 2nd Deliverable
Step 3: 
a)	Goal of the company:
Σκοπός μας είναι να βοηθήσουμε τους τυφλούς να αποφεύγουν εμπόδια (κινούμενα και σταθερά) σε χώρους τους οποίους δεν έχουν τη δυνατότητα να απομνημονεύσουν τη θέση κάθε αντικειμένου αλλά και υπάρχει πιθανότητα να έρθουν σε επαφή με κάτι κινούμενο που δε μπορούν να δουν (πχ αυτοκίνητα, πεζοί, ποδηλάτες και άλλα) με ένα προϊόν το οποίο θα είναι εύκολο στη χρήση και προσιτό σε τιμή.

b)	Users’ goals:
Οι χρήστες θέλουν ένα προϊόν που θα καλύπτει τις ανάγκες τους για ασφαλές περπάτημα στους εξωτερικούς χώρους. 

c)	Competitors: 
Υπάρχουν πολλά ανταγωνιστικά προϊόντα στην αγορά. Τα πιο συνηθισμένα είναι το γνωστό σε όλους μας άσπρο-κόκκινο ραβδί και οι εκπαιδευμένοι σκύλοι. Παρόλα αυτά, ύστερα από συνεντεύξεις που πήραμε, μάθαμε πως τα απλά ραβδιά δε βολεύουν τους χρήστες και δεν τους αποτρέπουν από συγκρούσεις με κινούμενα εμπόδια, ενώ ταυτόχρονα οι σκύλοι, αν και καλύτεροι, είναι πολύ ακριβοί για να μπορούν όλοι να τους αποκτήσουν.
   
Step 4:
Οι χρήστες θα ενεργοποιούν/απενεργοποιούν το προϊόν με φωνητική εντολή
Όταν θα βρίσκονται έξω, θα το χρησιμοποιούν για να αποφεύγουν εμπόδια. Για παράδειγμα:
o	Στα πεζοδρόμια θα αποφεύγουν πεζούς, τραπέζια, παγκάκια, δέντρα και άλλα
o	Στα πάρκα θα αποφεύγουν δέντρα, παιδιά που παίζουν, μπάλες και άλλα
o	Στο δρόμο (όταν το πεζοδρόμιο δεν έχει χώρο να περάσουν) θα αποφεύγουν όλα τα είδη οχημάτων
Step 5: 
στοιχεία διεπαφής: 1. κοντάρι με λουρί-χερούλι (που τυλίγεται γύρω από τον καρπό)
                                    2.Τρόπος έναρξης/απενεργοποίησης ρομπότ 
Ραβδί:
o	Ρόλος: ‘σύνδεση’ χρήστη με ρομπότ
o	Σχέση:  επαφής- κρατήματος
On/Off:
o	Ρόλος: έναρξη/κλείσιμο προϊόντος για εξοικονόμηση ενέργειας 
o	Σχέση: φωνητική σχέση με το χρήστη. Αφού ο χρήστης δε βλέπει, διευκολύνεται γιατί δε χρειάζεται να ψάξει κάποιο κουμπί/διακόπτη


# 3rd Deliverable 
step 6 and step 7:
Θα βρείτε φωτογραφίες για το storyboard και το πρωτότυπο και video αυτού ως φακέλους στο our report.
Κώδικας:
#include <Servo.h>          //Servo motor library. This is standard library
#include <NewPing.h> //Ultrasonic sensor function library. You must install this library
#include <L298N.h>


//our L298N control pins
const unsigned int IN1 = 7;
const unsigned int IN2 = 6;
const unsigned int ENA = 9; 

const unsigned int IN3 = 5;
const unsigned int IN4 = 4;
const unsigned int ENB = 10;

L298N motor1(ENA, IN1, IN2);
L298N motor2(ENB, IN3, IN4);


//sensor pins
#define trig_pin A1 //analog input 1
#define echo_pin A2 //analog input 2

#define maximum_distance 200
boolean goesForward = false;
int distance = 100;

NewPing sonar(trig_pin, echo_pin, maximum_distance); //sensor function
Servo servo_motor; //our servo name



void setup(){

  Serial.begin(9600);

  
  servo_motor.attach(10); //our servo pin

  servo_motor.write(90);
  delay(2000);
  distance = readPing();
  delay(100);
  distance = readPing();
  delay(100);
  distance = readPing();
  delay(100);
  distance = readPing();
  delay(100);
}

void loop(){

  int distanceRight = 0;
  int distanceLeft = 0;
  delay(50);
  Serial.print("Distance: ");
  Serial.println(distance);

      //moveForward(); 
      //delay(10000);
  
  if (distance <= 20){
    Serial.print("Mpika stin if");
    moveStop();
    delay(300);
    moveBackward();
    delay(400);
    moveStop();
    delay(300);
    distanceRight = lookRight();
    delay(300);
    distanceLeft = lookLeft();
    delay(300);

    if (distance >= distanceLeft){
      moveRight();
      delay(500);
      moveStop();
    }
    else{
      moveLeft();
      delay(500);
      moveStop();
    }
  }
  else{
    moveForward(); 
  }
    distance = readPing();
}

int lookRight(){  
  servo_motor.write(60);
  delay(500);
  int distance = readPing();
  delay(100);
  servo_motor.write(90);
  return distance;
}

int lookLeft(){
  servo_motor.write(120);
  delay(500);
  int distance = readPing();
  delay(100);
  servo_motor.write(90);
  return distance;
  delay(100);
}

int readPing(){
  delay(70);
  int cm = sonar.ping_cm();

  Serial.println(cm);
  return cm;
}

void moveForward()
{
    motor1.forward();
    motor2.forward();
}

void moveBackward()
{
    motor1.backward();
    motor2.backward();
}

void moveStop()
{
    motor1.stop();
    motor2.stop();
}

void moveRight()
{
   motor2.forward();
   motor1.stop();
}

void moveLeft()
{
   motor1.forward();
   motor2.stop();
}

//void servo move

# Conclusions


# Sources
