Welcome, you're about to start a trip of happy learning, you will learn how to create your own Web application with Python and Flask.
The video contains the whole preview of the content of the tutorial. By learning this chapter, you shall learn how to create a flask project, and run a simple flask web app on your own computer.

All the codes sed in the tutorial are presented on the Github. Although download from the github directly would save the steps of coding, but I strongly recommend you to type these codes in the first chapters. Once you are familiar with the Flask and the template web app, you can copy some of the code from the Github directly if the typing is so ***tedious.

At each chapter's beginning, I will provide three links to help you learn this chapter more smoothly. Click the *Browse* link will open the code repository page of corresponding Microblog project on Github, and there won't be any new code from the next chapter. And the *Zip* link will give you the zip file's download url. Click the *Diff* link, it's the change info of this chapter.

*The Github link of this chapter is [Browse](https://github.com/codingOuch/Flask_tutorial-translation/tree/master/Chapter%20I%20Hello%2C%20world!), [Zip], [Diff]*


# Install Python

pass

# Install Flask

pass

# "Hello, World" Flask App
Flask Webpage shows a simple template application with only five rows of codes. And I will give you a more complicated example, it will give you a very good base structure for writing a larger app.

The app will exist in a *package*. In Python, a sub-directory containing ```__init__.py``` file will be seen as a package that can be imported. When you import a package, the ```__init__.py``` will execute and define the attributes exposed by the package.

Now, let's create a new package called `app`, which will host the whole app. Remember to change back to the *microblog* directory and then run the code:
`$ mkdir app`
then create the `__init__.py`, type the following code:
```
from flask import Flask
app = Flask(__name__)
from app import routes
```
The script above only imports the class `Flask` from the flask, and create a web app object with this class. the `__name__` variables passed to the class Flask is a Python predefined variable, which is set to the name of the module in which it used. When related resources is needed to load, as the template I said in the [Chapter II] `Todo`, Flask will use this location as the 












