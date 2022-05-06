# CSML Modules

**Easy-to-use modules for the [CSML Engine](https://csml.dev)**

## Usage

To import these modules in your CSML code, you can use the public raw URL of the flow you would like to import as a module. Declare it as a dependency in your bot model and rebuild your bot. Then import it as a module by using the syntax `import myFunction from modules/nameOfModule`.

## Example

In this repository, we added a simple [buttons.csml](modules/buttons.csml) flow. You can add it as a dependency to your chatbot with the following raw github URL: https://raw.githubusercontent.com/CSML-by-Clevy/csml-modules/master/modules/buttons.csml.

```cpp
import YesNoButtons from modules/buttons

start:
  say Question("Do you like strawberries?", buttons=YesNotButtons("Yes, of course", "Not really"))
  hold
  say "Your answer was: {{event}}"
```

## Try it out

Create a free account on [CSML Studio](https://studio.csml.dev) and import a module in your hosted chatbot!
