## **GITHUB Branches**
#####**1. На локальном репозитории сделать ветки для:**
	- Postman
	- Jmeter
	- CheckLists
	- Bag Reports
	- SQL
	- Charles
	- Mobile testing

***Importante: the mandatory first command to make sure we are in main (or master) Directory***
```bash
git branch
```
1) **to create single branch** 
```bash
git branch MyBranchName
```
2) **to create multiple branches** 
```bash
git branch MyBranchName1 && git branch MyBranchName2 && etc
```
4) **to create single branch and switch in**
```bash
git checkout -b MyBranchName

5) **to delete branch in case of name changing** 
```bash
git checkout main
git branch -d MyBranchName
```
#####**2. Запушить все ветки на внешний репозиторий**
***Importante: each branch is pushing separately from the choosen branch lokation***
```bash
git checkout MyBranchName	// to switch to the branch we need to push
git push -u origin MyBranchName
```
#####**3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта**
```bash
git checkout BugReport
touch bug_report.txt
vim bug_report.txt
- enter TXT data:
[bug_report data](https://github.com/Olga-Ivasenko/JSON/blob/27513d59fa33744fef1ea328b0a6ed88cbe8a368/preferences.json)
```
#####**4. Запушить структуру багрепорта на внешний репозиторий**
```bash
git add .
git commit –m “bug report structure”
git push
```
#####**5. Вмержить ветку Bag Reports в Main**
```bash
git checkout main
git merge BugReports
```
#####**6. Запушить main на внешний репозиторий**
```bash
git checkout main		//if not there
git push -u origin MainDirectory
```
#####**7. В ветке CheckLists набросать структуру чек листа**
```bash
git checkout CheckLists
> checklist.txt
vim checklist.txt
- enter TXT data:
[Checklist data](https://github.com/Olga-Ivasenko/JSON/blob/27513d59fa33744fef1ea328b0a6ed88cbe8a368/preferences.json)
```
#####**8. Запушить структуру на внешний репозиторий**
```bash
git add .
git commit –m “check list structure”
git push
```
#####**9. На внешнем репозитории сделать Pull Request ветки CheckLists в main**
- go to GitHub YourRepositoryPage
- choose needed branch
![Chosing branch](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- push `Pull request` tab on above panel
![Pull request tab](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- push `New pull request` button colored green
![Create a request](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- push `New pull request` button colored green
![Create a request](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- in new window make sure the `base` is `main`, choose `compare` the branch you are merging in main
![Choose correct branch](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- find all files form choosen branch to be merged into `main`, push green colored button `Create pull request`
![Create a request](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- write down the name of your merge and push green colored button `Create pull request`
![Create a request](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- in new window make sure your merge does not have any conflicts, push `down arrow`near the `Merge pull request` green colored button
![Checking the conflicts](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- choose needed action depending the result you need (total branch merge or adding different part merge). In our case it should be `Create a new merge`
![Create a new merge](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)
- click on green colored button `Confirm merge``
![Merge finish](https://github.com/Olga-Ivasenko/JSON/blob/14e45b8cad289f91cc1002ad7302b7915268ba2a/edit_picture5.jpg)

#####**10. Синхронизировать Внешнюю и Локальную ветки Main**
```bash
git checkout main
git pull
```

