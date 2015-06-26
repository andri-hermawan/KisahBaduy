from flask import Flask, render_template
from flask.ext.mysql import MySQL

mysql = MySQL()
app = Flask(__name__)

# MySQL configurations
app.config['MYSQL_DATABASE_USER'] = 'root'
app.config['MYSQL_DATABASE_PASSWORD'] = ''
app.config['MYSQL_DATABASE_DB'] = 'latdbpython'
app.config['MYSQL_DATABASE_HOST'] = 'localhost'
mysql.init_app(app)

@app.route('/')
def home():
  return render_template('home.html')

@app.route('/about')
def about():
	return render_template('about.html') 

@app.route('/berita')
def berita():
	return render_template('berita.html')

@app.route('/kontak')
def kontak():
	return render_template('kontak.html')





if __name__ == '__main__':
  app.run(debug=True)

