Item                        Description
Base                        python:2.7-alpine
Work Directory              /app
Build Instruction           pip install -r requirement.txt
port                        80
launch command              gunicorn app:app -b 0.0.0.0:80


