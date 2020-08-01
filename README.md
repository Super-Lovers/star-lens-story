# Starry Story  documentation



## 📝 Table of Contents

* [Instructions for non-programmers](#instructions-for-non-programmers)
* [Instructions for programmers](#instructions-for-programmers)



### 📘 Instructions to modify and build story for non-programmers <a name = "instructions-for-non-programmers"></a>

1. First, clone the repository either by using a git client (sourcetree/git kraken), or by using the console.

       $ git clone https://github.com/Super-Lovers/star-lens-story

2. Open the repository and enter the ``dist`` folder and **copy all the contents** inside (images, fonts folders and project html file).
3. Go to the folder where Twine keeps its stories ("Documents > Twine > Stories" for me). If you don't know where that is, then:
4. Start the Twine application:

![](images/twine_app.png)

5. Go to **View** in the menu bar and press Show Story Library, which will open the folder for you:

![](images/twine_view.png)

6. Paste the contents you copied in step **2** into the Show Story Library folder from step **3 to 5**
7. Restart the Twine application and you should be able to see the story in the main menu:

![](images/twine_story.png)

8. You can now directly change the passages from the Twine application, however, you have to open the html file to play the story, rather than using Twine to play it. **You can change the story from the Application, but only play the story from the html file in the browser instead**.
9. Twine will create an html file from the story automatically named after the name of the story: 

![](images/folder_structure.png)

10. After you have updated the story using the Twine application and tested it from the browser, you have to now write the tested/finished passages to the repository we cloned from **step 1**. Going back to the folder where you cloned the repository from step 1, enter the folder ``src`` then ``story`` and move the contents from the passages you wrote and tested in the Twine application to those passages' respective files, replicating the same code they had in the Twine application you wrote with:

![](images/folder_story.png)

11. You can wait a minute for GitHub to build the application's new story and after that you can open it online from [here](https://super-lovers.github.io/star-lens-story/project.html) to see it and share it with others. **(If the changes don't appear right away, try F5 refreshing or CTRL-F5 refreshing)**.

    
### 📘 Instructions to modify and build story for programmers <a name = "instructions-for-programmers"></a>

1. First, clone the repository either by using a git client (sourcetree/git kraken), or by using the console.

       $ git clone https://github.com/Super-Lovers/star-lens-story

2. Download the Tweego compiler from (https://www.motoslave.net/tweego/)[https://www.motoslave.net/tweego/] and extract the contents.
3. Open the cloned repository and then open a git bash console from it by right clicking and selecting the Git Bash option:

![](images/folder_story.png)

4. In the console, run the tweego compiler with the following command:
    ````
    $ "C:\Users\Nikolay Ivanov\Downloads\tweego-2.1.1-windows-x64\tweego.exe" -o dist/project.html src/ --watch -t
    ````
    

The program will then continue running until you close it by typing CTRL-C. It will automatically detect changes in any of the files you modify in the ``src`` folder and it will build the project html file to the ``dist`` folder. Open it to look at your changes to the story.
