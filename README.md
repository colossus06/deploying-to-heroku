# deploying-to-heroku


When you're finished up with your software/app you need to do two things before deploying it to Heroku.

We need the following pre-requirements:
* `app.py`
* `Procfile`
* `requirements.txt file`
* A repository


Let's dive right in!

## 1
```
pip3 install gunicorn

```
or just write `gunicorn` on req.in file as show in the screenshot:

![image](https://user-images.githubusercontent.com/96833570/197387925-e92b4e57-0b71-4f6f-9f65-f1257a741bea.png)


## 2 
Create a `procfile` on the same level with your requirements.txt.
`touch Procfile` and write `web: gunicorn app:app`.

or 

`echo web: gunicorn app:app > Procfile`

Our current `app.py` folder looks like this:

```
from app import app

if __name__ == "__main__":
    app.run(debug=True)
```
![image](https://user-images.githubusercontent.com/96833570/197389586-e82ba9a9-f5ef-413a-82bb-b0d939051f6b.png)

## 3 

Create a repository and push your project.
