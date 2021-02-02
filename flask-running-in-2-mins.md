# flask-running-in-2-mins
### By Gontran Sion, the 2021-02-02.

# Flask running in 2 mins.
### By Gontran Sion, the 2021-02-01

From you project folder, start your environment and activate it.

''' python
python3.8 -m venv env
source env/bin/activate
'''

Install the flask lib and add it to the requirements file.

''' python
touch requirements.txt
pip install flask
pip freeze > requirements.txt
'''

let's add the flask app module with the simplest code and a fiel to lauch it.

''' python
touch run.py
mkdir module
cd module
touche __init__.py
'''

Add this code in run.py to lautch the app:

''' python
from module import app

if __name__ == '__main__':
    app.run(debug=True)
'''

now lwts edit the module with this code:

''' python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return 'Hello World!'

'''

and 'et voila !'
run it with 

 ''' python 
python run.py
 '''

 and copy past the link in your browser ... you should see Hello World!.

