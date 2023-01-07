Git-Github


<!-- WHY GIT -->

-Code share karne ke lliye
-Team can code together
-Purane code dekh skte
-Version management

Git is distributed version controlled system


<!-- To use git  -->

-Git ko allow karna version manage karne ke liye using----   git init
 dir -force(to see the files as well as hidden files)

 to see kon kon se changes hue hai file mein ya koi new file create hui hai -----    git status


 <!-- How to create versions -->
 Isme code mein changes kiye or main agge bhej skta hun
 Jab hun files add karenge to koi bhi added file phele untracked hita hai matalb git uspe dhyaan nhi deta

 jo jo files ko version mein final karna hai usko stagging area mein add karo
 to put a file in a stagging area mein we use------   git add (file name) (file2 name)
 or agar saari files bhejni hai to ------------    git add .     or       git add -A

 use "git rm --cached <file>..." to unstage/ ya fir ---  git restore --staged <file name>

 isko final version bnnae ke liye (staging area to final production product) we use -------------     git commit
 iske saath genrally hum ek msg daalte hai dekhne ke liye ko kya kaam kiyua tha hummien tab
 fir (i) dabakar insert kar skte hai
 vim seeeeeeeeeeeeeeeeeeeeeeee bahar aane ke liye esc ->:wq
 Agar vim ke bina commit karna hai to-------------   git commit -m   "msg" (to sarrri files jo stagging area mein hai woh commit hojayengi)

 abhi tak jo jo version add hue woh show honge  ---------------         git log

 latest version pe jaane ke liye  git checkout master
 jabbhi hum kaam karte hai humm= master branch pe kaaam ni karte hum karte hia branching

 <!-- Branching -->
 Master branch ka kaam hita hai production pe jana or isme kharab code ni ja skta
 to hum ek nyi branch dalte hai
 to creat barcnch phle hum check karte kon konsi current branches hai uske liye we use  ------------      git branch

 nyi branch bnne ke liye we use git branch [branch name]    (isse master ki saari files nyi branch pe aajyegi)

 agar dusri branch pe shift karna hai to git checkout {branch name}
 agar ab nyi branch ka saara code master pe daalna hai
 jabtak branch ke code ko merge ni karenge tab tak branch shift nhi karenge
 uske liye hum master pe aake merge karenge
 we do this with the help of ----------------------- git merge [branch name]

 Branch delete karne ke liye git branch -D [branch name] 

 nyi branch bnne ke or ussi time shift hojane ke liye
 git checkout -b [branch name]
 dono git branches ke beech mein diffrence karne ke liye -------------------   git diff [commit id]


<!-- Github  -->
It is a collection f repositries
the repo can be public or private

origin aapko btata hai git ko konse pe hummein code fekna hai
iske lye humare pass ek link hoga

git remote add origin url

origin dekhne ke liye
git remote show origin

there is somthing called upstream
iska matlb hai main 2 url rkh sakta hun fetch or push ke liye

