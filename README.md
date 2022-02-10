# ThisKeyword
Whenever JS program is run a global object is created(window), global execution context is created along with that execution context and this keyword is created. Global obejct is created even before JS engine enters to the GEC(Global Execution Context) and what Global object contains it contains eventHandlers, history,ScrollX,Window object(in the case of browser), localStorage and more..
\
even if Js file is empty there is nothing to execute JS engine still creates Global obect in the case of browser it's window.\
\
GEC- this is default execution context in which JS code start it's execution when the file first loads in the browser, GEC is created and it is pushed into the callstack, Everyhting in JS happens inside the GEC(global execution context).

first Javascript engine loads the JS file and parses the code then it enters into Global Execution Context that is the default execution context where JavaScript engine enters first.

After the parses of js code this is the default execution context where JS engine enters(Global Execution Context).Once the Js engine inside this global
execution context it creates 2 properties in the global memory by default the window object (in the case of browser) and this object.\
At the global level this keyword is equivalent to window object.\
***this===window***

**this Alone**
refers to the global object ***this===window***\
\
**this in method** refers to the owner of it's object\
const user={\
  firstName:"Varun",\
  lastName:"Kumar",\
  getFullName:function(){\
  console.log(`${this.firstName} ${this.lastName}`,**this**);\
}\
user.getFullName();\
output= Varun Kumar\
and this keyword will return a object

**Note** arrow function has no this keyword.


