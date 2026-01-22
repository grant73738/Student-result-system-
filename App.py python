from flask import Flask, render_template, request, redirect
import sqlite3

app = Flask(__name__)

def get_db():
    return sqlite3.connect("database.db")

@app.route("/")
def index():
    db = get_db()
    students = db.execute("SELECT * FROM student").fetchall()
    return render_template("index.html", students=students)

@app.route("/add_student", methods=["POST"])
def add_student():
    name = request.form["name"]
    matric = request.form["matric"]

    db = get_db()
    db.execute(
        "INSERT INTO student (name, matric_number) VALUES (?, ?)",
        (name, matric)
    )
    db.commit()
    return redirect("/")

if __name__ == "__main__":
    app.run(debug=True)
