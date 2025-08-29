1. a)getElementByid : 
     html er nirdishto id deoa element ke select kore object hisebe nei / return kore 
     <p id=p ></p>
     document.getElementByid("p")
   b)getElementsByClassName :
     html doc er class die nirdisto kora kono element ke select kore object hisab nei /return kore
     <p class =pp></p>
     document.getElementByClassName("pp")
   c)querySelector:
      css selector use kore jekono mil paoa element id / class prothom element ke return kore
      <p class =pp></p>
      <p class =pp></p>
      document.querySelector(".pp");
      sudhu prothom take return korbe
   d)querySelectorAll:
     <p class =pp></p>
     <p class =pp></p>
     css selector use kore sob mil paoa element id / class ke return kore
      document.querySelectorAll(".pp");
      
 2. a) notun upadan toiri kore :
      const newDiv = document.createElement("div");
    b) notu updan parent theke child sonnibesh kore:
       const container = document.getElementById("container");
        container.appendChild(newDiv); 

3. event bubbling holo ekti event handler er ekadhik eki upadan thakle sekhan e konta age konta pore kaj
   korbe seta thik kora . jemon parent er ta age kaj korbe naki chaild er ta .
   seta hote pare parent theke child er dik e dhap e dhap e trigger / logic kaj kora othoba child theke parent er dike
   logic kaj korano.
   kaj : eikhan child theke parent er ekti udahoron deoa holo :
   
    document.getElementById("child").addEventListener("click", function() {
    alert("Button clicked!");
    });

    document.getElementById("parent").addEventListener("click", function() {
    alert("Parent Div clicked!");
    });
   prothome child er ta show korbe pore parent er ta show korbe .

4.  Event Delegation holo parent element er event listener diye tar 
    child elements er events handle kora .

    karjokarita : a) sob child alada vabe handle korte hoi na
                  b) notun toiri hoa child o kaj kore

5. a) preventDefault() : browser er built in auto load/link click/ submission er somoy load ke bondho kore.
                         tarfole vitore kono condition ase ki na seta check hoi.
   b) stopPropagation(): event bubbling thamay .

