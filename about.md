 这是使用Github Issues写的第一篇博客，简单记录下搭建步骤以及期间遇到的几个问题。
 
 1. 新建一个仓库gitblog
    下载到本地
 2. 新建仓库G_KEY
    a. 新生成一个[github token](https://github.com/settings/tokens)，
    New personal access token (classic)
    scope勾选： repo、workflow、gist、user，
    生成后复制到一个安全的地方存储后面备用；
    b. 配置[Repository secrets](https://github.com/humyna/gitblog/settings/secrets/actions)
    settings--secrets and variables--Actions--new repository secrets,名称为G_KEY,值就是上面的github token
 
 注意：这个G_KEY会在后面的gene_readme.yml文件中使用
 
 3. 下载yihong0618开源的[这个项目](https://github.com/yihong0618/gitblog)，将其中除了feed.xml的文件全部copy到第一步项目中。
    a. BACKUP中只保留.gitkeep空文件，
    b. 修改gene_readme.yml文件，L11中分支名由master改成main;前面的G_KEY在这个文件配置(secrets.G_KEY)。
    c. 修改main.py文件，搜索master,改成main
 
 4.修改[workflow permissions](https://github.com/humyna/gitblog/settings/actions) ![image](https://private-user-images.githubusercontent.com/2505439/301553770-5d34862e-a7ca-458a-9e28-52b76df895d5.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjEyMTk3NzksIm5iZiI6MTcyMTIxOTQ3OSwicGF0aCI6Ii8yNTA1NDM5LzMwMTU1Mzc3MC01ZDM0ODYyZS1hN2NhLTQ1OGEtOWUyOC01MmI3NmRmODk1ZDUucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDcxNyUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA3MTdUMTIzMTE5WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9Y2UyOWFhZmZiZTY3NzdmN2FiZjE4NDM2MTI5NTNmMmMzN2M1YTAxMWRkMWJkZjNjYzJmZjY0ZWRkN2FjZWM4MiZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.Uk4ELDwlZNJ_Rh_lt6HxRQSTFs8Dg-9xNgmR4AzoiaE)
 
 如果不修改，在提交issue后，github actions执行报错 ![image](https://private-user-images.githubusercontent.com/2505439/301554548-e273a1c4-f217-414b-8329-27ad3fd8e605.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjEyMTk3NzksIm5iZiI6MTcyMTIxOTQ3OSwicGF0aCI6Ii8yNTA1NDM5LzMwMTU1NDU0OC1lMjczYTFjNC1mMjE3LTQxNGItODMyOS0yN2FkM2ZkOGU2MDUucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDcxNyUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA3MTdUMTIzMTE5WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9MGUzZjIxMTE3OTg0ZThiM2QwMjZlNjRmZmQ5NTJmMDQ2NGYyZGJhOTBmNTdmYjA1NTA4OWU0ZTQ1ODg5MDY1OCZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.oDR5gCC7WbN1qndEwCHZIJSjyCup9jubx4B3eViZNDY)
 
 5.初始化一些[labels](https://github.com/humyna/gitblog/labels)
 
 **至此基于issues个人博客就搭建完成了，可以愉快地写作了。**
 
 注意：提交issues，选择lable，github actions会被触发执行。

