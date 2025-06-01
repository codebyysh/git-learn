Git & Github
Commands in git
Firstly install git
CONFIG COMMANDS
1.
2.
3.
4.
5.
Git config —global user.name “Your name” — aap ho kon
aapka naam kya h
Git config — global user.email “email@gmail.com” — apka email
kya hh
Git config —global core.editor “code —wait” — agr git kbhi
bhi bolta h ki ye code shi nhi h to cons editor prr jaaye (jb bhi git error
dega tb VS code apne aap open ho jayega )
Git config —global core.autocrlf “input” — maan lo
Mac aur windows me alg alg trike se line end hoti hh to ye unko dono
ko sync krne ke kaam aata h
Git config —global -e ⸻⸻⸻⸻⸻—- agr kbhi value
edit krni hui to
Ab GIt apne khudke system me chlane ke liye hota h
U - untracked
A - added or staged
C - committed
Adding files
Stage them
Commit them
.gitignore file me us file ka name daal do
Rm -rf .git Age kisi bhi file ko ignore krna ho to use krte h aur is
agr git ko close krna ho to
●
Checkpoint bane ke liye kya kre
Git status -s ⸺ to know the current status of unstaged and
staged files (?? - mtlb git ko kuch nhi pta ⸻— A- added M- modified )
git log —oneline ---- to know the current status of saved points
….. checkpoint dekhne ke kaam aata h
git reset —hard (soft , hard , mixed ) HEAD~1/2/3/n — agr aapko
piche jana hh to
GIT BRANCHING
Git branch branchKaName branch feature/navbar)
Git branch Git switch feature/navbar h
Git switch main — branch bane ke kaam aata h (ex. Git
— sari branches dekhne ke kaam aata h
— branches me shift krne ke kaam aata
— main branch me aane ke kaam aata h
GIT MERGING and STASHING
Merge krne ke liye main branch me aana zaruri hh main se hi sari branch merge
kr skte hh
Git merge feature/navbar — merge krne ke liye
Ab agr dono branch ke same line me alg alg cheeze likhi hui hh to aapko
CONFLICT milega git ke dwara
Aur usko resolve krne ke liye apne paas 4 cheese hoti hh
1.
Accept current change ⸻⸻⸺ age aapko main brach ka code
rkhna h to ye kro
2.
Accept incoming change⸻⸻— agr aapko next branch ka code
rkhna h to ye kro
3.
Accept both changes ⸻⸻⸻ agr dono branch ka code rkhna
hh to ye krenge
4.
Compare changes
FAST FORWARD AND THREE WAY MERGE
This is three way merge
Head ko green se utha ke red pr rsh diya mtlb koi bhi commit nhi kiya direct hi
head ho utha ke nye branch pr le gyee isko hi kite h FAST FORWARD MERGING
HOW TO DELETE BRANCH
Git branch -d branchName
STASHING —
jab aap kisi branch me kam kr rhe hh aur aapne kuch code likha hh aur
usko aapne commit nhi kiya h but aap dusri branch me jaane ki koshish
krte ho to git aapko bolta h ki bhai saved nhi hh changes delete ho jayenge
gum chaahe to un changes ko delete hone de yaa fr un changes ko draft kr
skte h , jab bhi draft krenge to vo changes naa hi delete honge naa hi add
honge but beech me khi dale rhneg fir aap us branch me vapas aaye to vo
changes se apply kr skte h
Git stash ⸻⸻⸺ use kr skte h agr stash krna ho to
Git stash apply ⸻⸺ agr vapas code chaiye stash kra hua
THE STORY
jb bhi aap ek folder bnate h git ko kuch nhi pta aapke folder ke baare me
isliye aap waha git ko initialise krte hh
ab git ko permission mili hh to git aapke folder ko pehchaanta hai
to ab kyuki git kaam kr skta hh folder pr ab hm yhaa par tracked ,
untracked
modified staged and saved checkpoints create kr skte h
git kuch intresting cheeze kr skta hh jaise ki aap chaaye to kisi bhi
moment pr ye check kr skte ho aapki kitni files kis stage pr h
-> initialise kree
--> check kr skte ho aap konsi file kis stage me h --> git status -s
--> kitne saved points hh --> git log (—oneline (— graph))
--> branching
git status sirf unka status btayega jo files committed nhi h ya fr
commit hone ke baad change ho chuki ho
git status btata hh file ke changes ke bare me and uske state ke baare me
before commit or after commit
git status btata hh commit ke phle and baad ki stage
git log btata h saare comit histories
jab aap kisi branch me kam kr rhe hh aur aapne kuch code likha hh aur
usko aapne commit nhi kiya h but aap dusri branch me jaane ki koshish
krte ho to git aapko bolta h ki bhai saved nhi hh changes delete ho jayenge
gum chaahe to un changes ko delete hone de yaa fr un changes ko draft kr
skte h , jab bhi draft krenge to vo changes naa hi delete honge naa hi add
honge but beech me khi dale rhneg fir aap us branch me vapas aaye to vo
changes se apply kr skte h
GITHUB and COLLABORATION
COMMON STEPS
⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻⸻
Main bnda folder and initial files bnayega
Ab use GitHub pr daal de
Collaborators add krega
Saare bade us repo se cloning krenge
[VERY IMPORTANT] apni branch create krenge
Apna code use branch me likhenge
Complete hone prr commit kr denge and push kr denge
Inform krenge teammate ko about that commit
Merger bnda fetch krega and merge krega and repush kr dega
Yash jangid kr rha h ye sb kaam
Echo “# repoName” >> README.md
Git init
Git add . Git add filename ⸻⸻ agr sari files add krni ho to
⸻⸺ agr ek hi file add krni ho
to
Git commit -m “initial stage 0” ⸻⸻⸺ Phil stage commit
krne ke liye
Git remote add origin aapkiRepoKaLinkDo ⸻⸻— iss se pta lg jayega ki
sapka code upload kha krna h system se
Git push -u origin main
Yash kumawat kr rha h ye sb
CLONING
Git clone linkOfRepo
Git branch branchKaName ⸻—or⸻⸺ git switch -C branch_
name
Git switch branchkaName
Git add .
Git commit -m “added marquee effect ” ⸻⸻⸻— kumawat ne abhi
apne laptp pr checkpoint liya h
Git push -u origin branchKaName (featue/addedmarqueefftect)
Abhi tk Kumawat ne apna code push kr diya h
Ab jangid fetch krega us code ko
Git fetch ⸻⸻⸻⸺ branch fetch ho chuki h
Git branch ⸻⸻⸻ branch dikhne lg jayegi
Git switch branchName ⸻— yash jangid ke laptop prr same code dikhne
legs jo kumawat ne likha tha uske laptop prr
Jangid bhai code check krega and dekhega ki code shi ay kya agr shi ay to
Ab jangid apni main branch me aayega
Aur merge krega apne code me
Git merge branchName
(Ab ye merge ho chuka hh main code me yash kumawat bhai ka code but abhi
ye merge code sirf jangid ke laptop prr hi push nhi hua h GitHub prr to push
krna pdega )
Git push origin main ⸻⸻⸺ ab Sara code GitHub pr jaa chukka hh
Ab jangid ne to push kr diya hh GitHub prr but scene ye hua ki Abhi Kumawat ke
paas code nhi aaya neye wala merge wala code to kumawat ko ab pull krna
pdega ya fetch krna pdega
Kumawat kr rha h ye laptop pr
Git fetch
Git pull (fetch and merge ek sath ho jata h is se )
Ab vo sara code kumwat ke paas bei aa chuka h