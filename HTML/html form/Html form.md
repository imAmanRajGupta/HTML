# Html Form
1.Form are used to accept input from user.
2.To create Form in html we use <form></form> tag.
3.It is a container tag.
4.In html form , we are accepting input from user in an input field.
5.To create input field we use <input> tag. It is a non-container tag(un-pair tag).

# Attreibutes in Input Tag

1. Type: type attribute is used to specify which type of data we can accept in input field.

 <input type="_____">

 values:- 1) text    //name
          2) tel    //number
          3) email    //email id
          4) password     
          5) file multiple
          6) date    
          7) time
          8) datetime-local
          9) color
          10) range
          11) search
          12) url
          13) submit
          14) reset   //cancel
          15) number
          16) radio
          17) checkbox
          18) image
          19) button
          20) month
          21) week
          22) hidden

 # 2. NAME:-

  Name attribute is used to provide name to the input field.

  # 3. Value:-

  Value attribute is used to provide initial value to the input field.
              or
  Value attribute is used to target value inside an input field.

  # 4. Readonly:-

  It will  make the input field an readonly used can not change the value, but can access the input field.

  # 5. disabled:-

  It will make the input field as disabled user can not access the input  field.

  # 6. required:-

  It will make the input field as required to be filled . If input field is empty form will not be submitted.

  # 7. placeholder:-

  It is used to provided hint to the user.

  # 8. autofocus:-

  Whenever page reloads it will automatically focus an input field.

  # 9. size:-

  It is used to control the length of an input field.
     
     size="_______"value=30(number)

  # 10. maxlength:-

   The maxlength attribute specifies the maximum number of charcters allowed in an input field.
   maxlength="__________" value=16(number)

  # 11. minlength:-

   The minlength attribute specifies the minimum number of characters allowed in an input field.
     
     minlength="___"value=2(number)

  # 12. max:=

   1. It is used with type=number,rannge
   2. Max attribute specifies the maximum value of an input field.

    max="____" value=10 (number)

  # 13. min:-

   1. It is used with type=number,range
   2. Min attribute specifies the minimum value of an input field.

    min="____" value=5(number)

  # 14. autocomplete:-

    The autocomplete attribute specifies if browsers should try to predict the value of an input field or not.

    autocomplete="___" value=on| off

  # 15. step:-

    Step Attribute is used to  set the discrete step size of an input tag. The default stepping value for number inputs is 1.

    IT WORKS WITH:-
     number
     range
     date
     datetime-local
     month
     time
     week

   # 16. accept:-

    Accept Attribute is used to specify the file types that the input field can accept.

    accept="___"

     1. audio/*: The User can pick all sound files.
     2. video/*: The user can pick all video files.
     3. image/*: A valid media type,with no parameters.
     4.  .png


   # Label Tag:-
 
    1. Label tag is used to connect text with the input field.
    2. The text we want to connect we have to write within label tag.
    3. It is container tag.
    4. In input tag,we have to use id attribute and that id's value we have to pass to label's for attribute.
    5. Whenever use click on that text respective input field will be focused.

      # Syntax:-
      <label for="username">Name</label>
      <input type="text" id="username>


   # Fieldset Tag:-

    1. Fieldset Tag is used to group form control and it will create one box around the group.
    2. It is container Tag.
    3. Fieldset Tag we have to write with in form Tag.


   # Legend Tag:-

    1. It is container Tag.
    2. To provide title or caption to the fieldset we use legend Tag.
    3. Legend tag we have to write with in fieldset Tag.

     # Syntax:-

     <form action="">
     <fieldset>
     <legend> Registration form</legend>
     <label for="username">Name</label>
     <input type="text" id="username">
     <br><br>
     </fieldset>
     </form>


   # select Tag:-

    1. It is container Tag.
    2. It is used to create dropdown list.
    3. To create dropdown list we use select tag.
    4. Here we are providing multiple options to the user from these option user  can select only one option.
    5. To create option we use option tag.
    6. It is container tag.

     # Syntax:-

      <select name="State-name" id="">
      <option value="" select disabled>---Select State Name---</option>
      <option value="delhi">Delhi</option>
      <option value="mumbai">Mumbai</option>
      <option value="uttar pardesh">Uttar pardesh</option>
      <option value="Haryana">harayana</option>
      <option value="Bihar">Bihar</option>
      </select>


    # Disadvantage of Select Tag:-

      1. The main disadvantage of the select tag is that it limits the user's input options to the predefined list of options provided by the developer using the option tags.
      2. The user cannot enter  any text of their choice or customize the options available in the list.

   # DataList Tag: Autocomplete List/ Suggestion List
    1. The Datalist Tag is introduced in Html5.
    2. The Html datalist tag is used to provide an autocomplete feature on the form element.
    3. Datalist tag is a container tag.
    4. It is block level element.
    5. It is used to provide a list of predefined options to the users.
    6. Datalist tag is used to create suggestion list or autocomplete list.
    7. The <datalist> tag contains a set of <option> tags that define the options in the list.
    8. We are binding the suggestion list with the input field, for this we have to provide 'list' attribute in the input tag and     'id' attribute in the datalist tag, this same 'id' we have to provide in the 'list' attribute of input tag.
    9. Whenever the user inputs in the input field related suggestions are displayed.
    10. The advantage of using the datalist tag is that it allows users to enter values that are not present in the options list

    11. syntax:- 

   <input type="text" list="state-name" placeholder="Enter state name">

   <datalist id="state-name">
    <option value="Delhi"></option>
    <option value="Mumbai"></option>
    <option value="Uttar Pradesh"></option>
    <option value="Bihar"></option>
   </datalist>


   # Textarea:-
    It is container.
    It is used to accept multi line input from the user.
    # note:- when content is more inside the textarea, it will automatically create scroll bar.

    # Attributes of Textarea:-
     rows:- rows attribute is used to provide the dimension of height.
     cols:- cols attribute is used to provide the dimension of width.
     
    # syntax:-
     <textarea rows="10" cols="30" name="" id=""></textarea>

   
   # Diff between input type submit and button tag?
     
                 input type:"submit"                                                      Button tag
      
      1. It is non coitainer tag.                                           1. It is a container tag.

      2. It will always try to connect to the server if server              2. It will not try to connect to the server.
         is there it will send the data.
      
      3. It will reload the page.                                           3. It will also reload the page but we can prevent using js.

      4. It is not fully compatible with the js.                            4. It is fully compatible with js.

      5. In Input type submit ,we cannot use any other content              5. In button submit ,we can use image or any other content 
         to create submit button.                                              to create a button. (anyother content-audio,vedio etc.)

   
   # Diff between id and class?

                     ID(#)                                                                  Class(.)
      1. It is use to target element uniquely.                              1. It is use to target multiple elements at a time.

      2. Multiple elements cannot have same id                              2. Multiple elements can have same class.
                                              
        Ex-  <p id="p tag-1">Paragraph-1</p> //same id is                      Ex-  <p class="p tag">Paragraph-1</p> //same class 
             <p id="p tag-1">Paragraph-2</p>   not allowed                          <p class="p tag">Paragraph-2</p>   names allowed

      3. One element can have only one id(single id).                       3. One element can have multiple classes.
        Ex-  <div id="div-1  tag-1">div tag</div>                              Ex- <div class="div-1 tag-1">Div tag</div>
             // It should be single only.                                           // Multiple class value allowed.

      4. To target the element using id in css ,we use                      4. To target an element using class in css ,we use
         (#)hash operator.                                                     (.) operator.

      5. It is a global attribute we can use in any tag.                    5. It is a global attribute we can use in any tag.