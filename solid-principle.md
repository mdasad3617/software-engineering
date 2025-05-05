## The SOLID Principles
https://daedtech.com/solid-principles-real-life/

### What are SOLID principles in programming?
SOLID principles are the set of software design principles used by software engineers in object-oriented software development to follow, scale and maintain a proper structure to the codes & programming. SOLID is a popular set of SOLID is an acronym that stands for five key design principles: single responsibility principle, open-closed principle, Liskov substitution principle, interface segregation principle, and dependency inversion principle.

The SOLID principles were developed by Robert C. Martin in a 2000 essay, “Design Principles and Design Patterns,” although the acronym was introduced later by Michael Feathers. As successful software changes, it becomes increasingly complex. Software becomes rigid, fragile, immobile, and viscous without good design principles. The SOLID principles were developed to combat these problematic design patterns.



### What is the importance of SOLID principles?
These five principles help us understand the need for certain design patterns andsoftware architecture in general. SOLID principles aim at reducing the dependencies of software engineers. As if they know and understand the basic architecture & design principles, it'll be easier for them to change or edit codes and alter a few changes if required. 

Additionally, SOLID principles enable engineers to make designs easier to understand, maintain, and extend. Ultimately, using these design principles makes it easier for software engineers to avoid issues and to build adaptive, effective, and agile software.
‍

### What is Object-oriented programming (OOP)? 
Object-oriented programming (OOP) is a modeling system and one of the classifications of programming languages built on the concept of "objects" which can contain data and code. Where "data" denotes fields, attributes, or properties and "code" is referred to as the methods or procedures. 

Object-oriented programming is about modeling a system as a collection of objects, which each represent some particular aspect of the system. Objects contain both functions (or methods) and data. An object provides a public interface to other code that wants to use it, but it maintains its private internal state: which means that other parts of the system don't have to care about what is going on inside the object. Object-oriented programming is faster and easier to execute and provides a clear structure for the programs. 


## The SOLID Principles
S — Single Responsibility
O — Open-Closed
L — Liskov Substitution
I — Interface Segregation
D — Dependency Inversion


### S is for Single Responsibility Principle
The single responsibility principle (SRP) asserts that a class or module should do one thing only.  Now, this is kind of subjective, so the principle is reinforced with the heuristic that the class or module should have only one reason to change.

By way of counter-example, consider a class that opens a connection to the database, pulls out some table data, and writes the data to a file.  This class has multiple reasons to change: adoption of a new database, modified file output format, deciding to use an ORM, etc.  In terms of the SRP, we’d say that this class is doing too much.

In your day to day life, picture those “duck” vehicles you see occasionally in some lakeside towns.  They’re street legal and water-capable, so a duck tour affords you the unique and surreal experience of being in a ‘car’ that gets to the edge of the water and just keeps going.  Fun, right?


And yet, you don’t see a whole lot of them.  There are millions of families out there that own both cars and boats, and there are very few families that buy these ducks.  Do you know why?  It’s most likely because no one wants to be unable to drive to work because their boat rudder is broken.  Ducks are fun, but they’re also a great example of the pitfalls that the SRP can help you avoid.


### O is for Open/Closed Principle
The Open/Closed Principle states that code entities should be open for extension, but closed for modification.  To put this more concretely, you should write a class that does what it needs to flawlessly and not assuming that people should come in and change it later.  It’s closed for modification, but it can be extended by, for instance, inheriting from it and overriding or extending certain behaviors.  An example of running afoul of the open closed principle would be to have a switch statement somewhere that you needed to go in and add to every time you wanted to add a menu option to your application.

A great example of this in real life is sitting in your pocket in the form of a smart phone.  All such phones have app stores and these app stores let you extend the base functionality of the phone.  Sure, it ships with the basics: camera operation, actual calls, text messages, etc.  But via the app store, you can extend the phone’s capabilities to allow you to manage your todo list, play inane video games, and even serve as a flashlight or wireless access point.

The mechanism that allows you to do this is purely one of extension, however.  It’s not as though Apple, Google, and Microsoft put the OS source code up on github and invite you to dive in and start building games and flashlight functionality.  Rather, they make the core phone functionality closed for modification and they open it to extension.

### L is for Liskov Substition Principle
The Liskov Substition Principle (LSP) is the one here that is most unique to object oriented programming.  The LSP says, basically, that any child type of a parent type should be able to stand in for that parent without things blowing up.

In other words, if you have a class, Animal, with a MakeNoise() method, then any subclass of Animal should reasonably implement MakeNoise().  Cats should meow, dogs should bark, etc.  What you wouldn’t do is define a MuteMouse class that throws IDontActuallyMakeNoiseException.  This violates the LSP, and the argument would be that this class has no business inheriting from Animal.

To picture this, imagine cooking yourself a stew.  If you’re anything like me, you’d only put things in there that were edible because you would want to eat the stew without picking through each bite, asking yourself repeatedly, “is this edible?”

### I is for Interface Segregation Principle
The Interface Segregation Principle (ISP) says that you should favor many, smaller, client-specific interfaces over one larger, more monolithic interface.  In short, you don’t want to force clients to depend on things they don’t actually need.  Imagine your code consuming some big, fat interface and having to re-compile/deploy with annoying frequency because some method you don’t even care about got a new signature.

To picture this in the real world, think of going down to your local corner restaurant and checking out the menu.  You’ll see all of the normal menu mainstays, and then something that’s just called “soup of the day.”  Why do they do this?  Because the soup changes a lot and there’s no sense re-printing the menus every day.  Clients that don’t care about the soup needn’t even be concerned, and clients that do use a different interface — asking the server.

### D is for Dependency Inversion
The Dependency Inversion Principle (DIP) encourages you to write code that depends upon abstractions rather than upon concrete details.  You can recognize this in code you read by looking for a class or method that takes something generic like “Stream” and performs operations on it, as opposed to instantiating a specific Filestream or Stringstream or whatever.  This gives the code in question a lot more flexibility — you can swap in anything that conforms to the Stream abstraction and it will still work.

To visualize this in your day to day, go down to your local store and pay for something with a credit card.  The clerk doesn’t examine your card and get out the “Visa Machine” after seeing that your card is a Visa.  He just takes your card, whatever it is, and swipes it.  Both you and the clerk depend on the credit card abstraction without worrying about specifics.

And, That’s SOLID!



----------------translation---------------

# The SOLID Principles
[Link to Article](https://daedtech.com/solid-principles-real-life/)

## SOLID principles kya hai programming mein?
SOLID principles ek set hai software design principles ka jo software engineers use karte hain object-oriented software development mein, taaki code aur programming ka structure proper, scalable aur maintainable rahe. SOLID ek acronym hai jo five key design principles ke liye stand karta hai: **single responsibility principle**, **open-closed principle**, **Liskov substitution principle**, **interface segregation principle**, aur **dependency inversion principle**.

SOLID principles ko **Robert C. Martin** ne 2000 mein ek essay “Design Principles and Design Patterns” mein develop kiya, though acronym baad mein **Michael Feathers** ne introduce kiya. Jab software successful hota hai aur change hota hai, toh yeh complex ho jata hai. Agar good design principles nahi hote, toh software **rigid**, **fragile**, **immobile**, aur **viscous** ho jata hai. SOLID principles is problem ko tackle karne ke liye develop kiye gaye.

## SOLID principles ki importance kya hai?
Yeh five principles humein samajhne mein help karte hain ki certain design patterns aur software architecture ki zarurat kyun hai. SOLID principles ka aim hai software engineers ke **dependencies** ko reduce karna. Agar unhe basic architecture aur design principles pata hote hain, toh code change ya edit karna, ya thodi si changes karna easier ho jata hai.

Iske alawa, SOLID principles engineers ko designs banane mein help karte hain jo **samajhne**, **maintain karne** aur **extend karne** mein aasan hote hain. Ultimately, in design principles ka use karne se software engineers ke liye issues avoid karna aur **adaptive**, **effective**, aur **agile** software build karna easier ho jata hai.

## Object-oriented programming (OOP) kya hai?
Object-oriented programming (OOP) ek **modeling system** hai aur programming languages ka ek classification hai jo **“objects”** ke concept pe based hai, jisme **data** aur **code** dono ho sakte hain. Yahan “data” ka matlab hai **fields**, **attributes**, ya **properties** aur “code” ka matlab hai **methods** ya **procedures**.

Object-oriented programming ka matlab hai ek system ko **objects ke collection** ke roop mein model karna, jisme har object system ke kisi **particular aspect** ko represent karta hai. Objects mein **functions (ya methods)** aur **data** dono hote hain. Ek object dusre code ke liye **public interface** provide karta hai jo usse use karna chahta hai, lekin apna **private internal state** maintain karta hai: iska matlab hai ki system ke dusre parts ko is baat ki chinta nahi karni padti ki object ke andar kya chal raha hai. Object-oriented programming **faster** aur **easier execute** hoti hai aur programs ke liye **clear structure** provide karti hai.

## The SOLID Principles
- **S** — Single Responsibility
- **O** — Open-Closed
- **L** — Liskov Substitution
- **I** — Interface Segregation
- **D** — Dependency Inversion

### S matlab Single Responsibility Principle
Single responsibility principle (SRP) ka kehna hai ki ek **class** ya **module** ko sirf **ek kaam** karna chahiye. Yeh thoda **subjective** hai, isliye is principle ko reinforce kiya jata hai is heuristic se ki class ya module ke **change ka sirf ek reason** hona chahiye.

Counter-example ke roop mein, ek class socho jo **database ka connection** open karta hai, **table data** pull karta hai, aur data ko **file mein write** karta hai. Is class ke change ke **multiple reasons** hote hain: **new database** adoption, **file output format** change, **ORM** use karne ka decision, etc. SRP ke terms mein, hum kehenge ki yeh class **bahut zyada kaam** kar rahi hai.

Aapke daily life mein, socho un **“duck” vehicles** ke baare mein jo kabhi kabhi **lakeside towns** mein dikhte hain. Yeh **street legal** aur **water-capable** hote hain, toh duck tour mein aapko ek **unique aur surreal experience** milta hai jab aap ek **‘car’** mein hote ho jo **water ke edge** tak jati hai aur wahi chalta rehta hai. **Mazedaar**, na?

Lekin, aap inhe zyada nahi dekhte. **Lakhs families** ke paas **cars** aur **boats** dono hote hain, lekin bahut kam families yeh **ducks** khareedti hain. Jaante ho kyun? Most likely isliye kyunki koi nahi chahta ki **boat rudder** kharab hone ki wajah se woh **kaam pe drive** na kar sake. Ducks **fun** hote hain, lekin yeh bhi SRP ke **pitfalls** avoid karne ka ek **great example** hain.

### O matlab Open/Closed Principle
Open/Closed Principle ka kehna hai ki **code entities** ko **extension ke liye open** hona chahiye, lekin **modification ke liye closed**. More concretely, aapko aisa **class** likhna chahiye jo apna kaam **perfectly** kare aur yeh assume na kare ki log baad mein aake isme **change** karenge. Yeh **modification ke liye closed** hai, lekin isse **extend** kiya ja sakta hai, jaise **inheritance** ke through ya certain **behaviors** ko **override** ya **extend** karke. Open closed principle ke against ek example hoga ek **switch statement** jisme aapko har baar jana padta hai aur **add** karna padta hai jab aap apne **application** mein ek **menu option** add karna chahte ho.

Iske real life ka ek **great example** aapke **pocket** mein hai — **smart phone**. Sabhi phones mein **app stores** hote hain aur yeh app stores aapko phone ke **base functionality** ko **extend** karne dete hain. Sure, yeh **basics** ke saath ship hota hai: **camera operation**, **actual calls**, **text messages**, etc. Lekin **app store** ke through, aap phone ke **capabilities** ko extend kar sakte ho, jaise **todo list** manage karna, **inane video games** khelna, ya **flashlight** ya **wireless access point** ke roop mein use karna.

Yeh **mechanism** purely **extension** ka hai, lekin. Aisa nahi hai ki **Apple**, **Google**, aur **Microsoft** OS ka **source code** github pe daal dete hain aur aapko **invite** karte hain ki aake **games** ya **flashlight functionality** build karo. Balki, woh **core phone functionality** ko **modification ke liye closed** rakhte hain aur **extension ke liye open**.

### L matlab Liskov Substitution Principle
Liskov Substitution Principle (LSP) yahan sabse **unique** hai object-oriented programming ke liye. LSP basically kehta hai ki koi bhi **parent type** ka **child type** parent ke liye **stand in** kar sakna chahiye bina kisi cheez ke **blow up** hone ke.

Dusre shabdon mein, agar aapke paas ek class hai, **Animal**, jisme ek **MakeNoise()** method hai, toh Animal ka koi bhi **subclass** reasonably MakeNoise() ko **implement** karna chahiye. **Cats** ko **meow** karna chahiye, **dogs** ko **bark** karna chahiye, etc. Aap kya nahi karenge woh hai ek **MuteMouse** class define karna jo **IDontActuallyMakeNoiseException** throw karta hai. Yeh LSP ko **violate** karta hai, aur argument hoga ki is class ka Animal se **inherit** karna ka koi **business** nahi hai.

Ise picture karne ke liye, socho ki aap ek **stew** cook kar rahe ho. Agar aap mere jaise ho, toh aap usme sirf wahi cheezein daaloge jo **edible** hain kyunki aap stew ko **khaana** chahte ho bina har **bite** ko check kare ki “yeh **edible** hai kya?”

### I matlab Interface Segregation Principle
Interface Segregation Principle (ISP) kehta hai ki aapko **many**, **smaller**, **client-specific interfaces** ko prefer karna chahiye over ek **larger**, **monolithic interface** ke. Short mein, aap nahi chahte ki **clients** ko un cheezon pe **depend** karna pade jo unhe **actually chahiye nahi**. Socho aapka **code** ek **bada**, **fat interface** consume kar raha hai aur aapko **annoying frequency** ke saath **re-compile/deploy** karna padta hai kyunki koi **method**, jiske baare mein aapko **parwah** bhi nahi, uska **signature** change ho gaya.

Real world mein isse picture karne ke liye, socho apne **local corner restaurant** ke **menu** ke baare mein. Aapko **normal menu mainstays** dikhenge, aur phir kuch jo bas **“soup of the day”** kaha jata hai. Yeh kyun karte hain? Kyunki **soup** bahut **change** hota hai aur har roz **menu re-print** karne ka koi **sense** nahi hai. Jo **clients** soup ke baare mein **care** nahi karte, unhe iski **chinta** nahi karni padti, aur jo karte hain, woh **alag interface** use karte hain — **server** se poochke.

### D matlab Dependency Inversion
Dependency Inversion Principle (DIP) aapko **encourage** karta hai ki aap aisa **code** likho jo **abstractions** pe depend kare, na ki **concrete details** pe. Aap isse **code** mein **recognize** kar sakte ho by looking for a **class** ya **method** jo kuch **generic** leta hai jaise **“Stream”** aur uspe **operations** perform karta hai, instead of **specific Filestream** ya **Stringstream** ya whatever **instantiate** karne ke. Yeh code ko **bahut zyada flexibility** deta hai — aap koi bhi cheez **swap in** kar sakte ho jo **Stream abstraction** ke saath **conform** karti hai aur yeh **kaam** karega.

Ise **daily life** mein visualize karne ke liye, apne **local store** pe jao aur **credit card** se kuch **pay** karo. **Clerk** aapka **card** examine nahi karta aur **“Visa Machine”** nikal kar nahi laata yeh dekhne ke baad ki aapka card **Visa** hai. Woh bas aapka **card**, jo bhi ho, leta hai aur **swipe** karta hai. Aap aur **clerk** dono **credit card abstraction** pe **depend** karte ho bina **specifics** ki chinta kiye.

## Aur, yeh hai SOLID!
