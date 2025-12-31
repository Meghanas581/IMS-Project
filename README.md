# app.py
from flask import Flask, render_template, request, redirect, url_for, session
import json, os


app = Flask(__name__)
app.secret_key = 'secret123'


DATA_FILE = 'inventory.json'
USERS_FILE = 'users.json'