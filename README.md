# ASH Bundler

to use, call *bundle_and_write()* with 2 or 3 arguments.<br>
### **argument 1**: path to the script you want to bundle.
   WARNING: this path needs to be **relative to your mafia folder.**<br>
   This means this value will always be either "relay/[...].ash" or "scripts/[...].ash"<br>
    example: "relay/relay_TourGuide.ash"<br>

### **argument 2**: path to the soon-to-be-created bundled file.<br>
   Can either be absolute or relative.<br>
    if relative, the reference is the folder in which *THIS SCRIPT* was ran.<br>
        examples: `C:/Users/Keith/Documents/my_precious/my_script.ash`<br>
          or      `my_script.ash`<br>

### **argument 3 (optional)**: the path to *REACH YOUR MAFIA FOLDER*
   Can be either absolute or relative<br>
   if you run this script from within your mafia folder, don't submit anything here.<br>
   Otherwise, this is the folders that this script has to go through to reach your mafia folder<br>
    (or whatever folder contains the "scripts" and/or "relay" folder(s) containing your scripts to import)<br>



#### EXAMPLE:
   - you run this program from your *DESKTOP*
   - you want to put the result in *C:/Users/Me/Desktop/Sekrits/my_bundled_script.ash*
   - your script is at *C:/Users/Me/Desktop/Games/Actually_entertaining_games/KoLMafia/scripts/my_script.ash*

   In the command line, you would do:<br>
       `C:\Users\Me\Desktop>  py Bundle_ASH_script.bundle_and_write( 'scripts/my_script.ash' , 'Sekrits/my_bundled_script.ash' , 'Games/Actually_entertaining_games/KoLMafia/' )`<br>

   Another way to do it would be to put, at the end of this file:<br>
       `bundle_and_write( 'scripts/my_script.ash' , 'Sekrits/my_bundled_script.ash' , 'Games/Actually_entertaining_games/KoLMafia/' )`<br>
   and then run, in the command line:<br>
    `C:\Users\Me\Desktop>  py Bundle_ASH_script`