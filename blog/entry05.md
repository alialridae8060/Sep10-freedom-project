# Entry 5
##### $/29/2025

### Okay I´ve reached the midway point in the freedom project and today I will talking about everything I´ve learned about my tool css variables.I learned a lot so instead of telling you all directly I will show all my notes of what I´ve learned so far.Here we go:
## <h1>What I learned about CSS Varaibles from 3/17/2025 to 3/24/2025.</h1>
 ### <ul>
  ## <li>3/17/2025</li>
  ##  <li>First of all CSS Variables is a nickname to Custom properties and is also called cascading variables.</li>
  ##          <li>In CSS variables you can declare a custom property by using the @property rule and/or the two dashes rule like this --</li>
    <li> section {
       --main-bg-color: blue n;
      }
         </li>
            <li>Also you can do the same thing for the logo of your wbesite.</li>
            <li>@property --logo-color {
                syntax: "<color>";
                inherits: false;
                initial-value: #c0ffee;
              }
              </li>
              <li>Here is what can yo with the background.</li>
              <li>
                details {
                background-color: var(--main-bg-color);
              }
              </li>
              <li>When coded correctly local variables such as the color blue would overide the global variable red.
                :root {
                  --blue: #1e90ff;
                  --white: #ffffff;
                }

                body {
                  background-color: var(--blue);
                }

                h2 {
                  border-bottom: 2px solid var(--blue);
                }

                .container {
                  color: var(--blue);
                  background-color: var(--white);
                  padding: 15px;
                }

                button {
                  --blue: #0000ff; /* local variable will override global */
                  background-color: var(--white);
                  color: var(--blue);
                  border: 1px solid var(--blue);
                  padding: 5px;
                }
              </li>
              <li>If a variable is used at only a singal place it becomes the new local color.
                :root {
                  --blue: #1e90ff;
                  --white: #ffffff;
                }

                body {
                  background-color: var(--blue);
                }

                h2 {
                  border-bottom: 2px solid var(--blue);
                }

                .container {
                  color: var(--blue);
                  background-color: var(--white);
                  padding: 15px;
                }

                button {
                  --button-blue: #0000ff; /* new local variable */
                  background-color: var(--white);
                  color: var(--button-blue);
                  border: 1px solid var(--button-blue);
                  padding: 5px;
                }
              </li>
              <li>CSS variables have access to DOM which means they can be changed with Javascript.
                <script>
                 // Get the root element
                  var r = document.querySelector(':root');

                  // Create a function for getting a variable value
                  function myFunction_get() {
                    // Get the styles (properties and values) for the root
                    var rs = getComputedStyle(r);
                    // Alert the value of the --blue variable
                    alert("The value of --blue is: " + rs.getPropertyValue('--blue'));
                  }

                  // Create a function for setting a variable value
                  function myFunction_set() {
                    // Set the value of variable --blue to another value (in this case "lightblue")
                    r.style.setProperty('--blue', 'lightblue');
     }
    </script>
   </li>
 </ul>
 
 ## There are more coming:
   ## <h1>What I learned about CSS Varaibles from 3/17/2025 to 3/24/2025.</h1>

  ## <ul>
   ## <li>3/17/2025</li>
  ## <li>First of all CSS Variables is a nickname to Custom properties and is also called cascading variables.</li>
  ## <li>In CSS variables you can declare a custom property by using the @property rule and/or the two dashes rule like this --</li>
            <li> section {
                --main-bg-color: blue n;
              }
              </li>
            <li>Also you can do the same thing for the logo of your wbesite.</li>
            <li>@property --logo-color {
                syntax: "<color>";
                inherits: false;
                initial-value: #c0ffee;
              }
              </li>
              <li>Here is what can yo with the background.</li>
              <li>
                details {
                background-color: var(--main-bg-color);
              }
              </li>








        </ul>

## Finally there is:
body { background-color: #ff4b1e; }

h2 { border-bottom: 4px solid #ff711e; }

.container {
  color: #ff5e1e;
  background-color: #ef4511;
  padding: 20px;
}

button {
  background-color: #f08307;
  color: #ff2d1e;
  border: 4px solid #ff311e;
  padding: 10px;
}
:root {
  --red: #ff261e;
  --orange: hsl(25, 94%, 50%);
}

body { background-color: var(--orange); }

h2 { border-bottom: 6px solid var(--orange); }

.container {
  color: var(--orange);
  background-color: var(--orange);
  padding: 20px;
}

button {
  background-color: var(--red);
  color: var(--orange);
  border: 4px solid var(--red);
  padding: 10px;
}
:root {
  --red: #ed6d64;
  --orange: #f17f0d;
}

body { background-color: var(--red); }

h2 { border-bottom: 6px solid var(--orange); }

.container {
  color: var(--red);
  background-color: var(--orange);
  padding: 20px;
}

button {
  background-color: var(--orange);
  color: var(--red);
  border: 4px solid var(--red);
  padding: 10px;
}
p {
  bacground-color: var(--green)
  color: var(--blue);
  border: 8px solid var(--blue);
  padding: 11px;
}

## So this what I´ve learned about CSS variables.Sorry if it isn the height you my bviewers envisioned but here is everything I learned.So I hope you all enjoyed reading my vlog and I hope write to you all in my next vlog.Bye.

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
