# GIT_branch
1. На локальном репозитории сделать ветки для:

- Postman: git branch Postman
- Jmeter: git branch Jmeter
- CheckLists: git branch  CheckLists
- Bag Reports; git branch BagReports
- SQL: git branch SQL
- Charles: git branch Charles
- Mobile testing:  git branch  MobileTesting
$ git branch
  BagReports
  Charles
  CheckLists
  Jmeter
  MobileTesting
  Postman
  SQL
* main
 
2. Запушить все ветки на внешний репозиторий:  git push -u origin  BagReports Charles CheckLists Jmeter MobileTesting Postman SQL
3. В ветке BagReports сделать текстовый документ со структурой баг репорта
 git checkout BagReports
touch structureBagReport.txt
cat >> structureBagReport.txt
ID:
Reporter:
Severity:
Priority:
Status:
Product Build:
Reproducibility:
Platform:
OS:
OS Version:
Resolution:
Summary:
Description:
Steps To Reproduce:
Actual result:
Expected result:
Additional Information:
Attached Files:

4. Запушить структуру багрепорта на внешний репозиторий:
 git add structureBagReport.txt
 git commit -m "add structure bagreport"
5. Вмержить ветку Bag Reports в Main
git checkout main
git merge BagReports -m "merge add"
6. Запушить main на внешний репозиторий:  git push
7. В ветке CheckLists набросать структуру чек листа
touch myCheckListst.txt
cat >> myCheckListst.txt
8. Запушить структуру на внешний репозиторий
git add myCheckListst.txt
git commit -m "added check List"
git push
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main : compare & pull request
10. Синхронизировать Внешнюю и Локальную ветки Main
git checkout main
git fetch
git pull


