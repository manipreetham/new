
# Qgenie Project - Setup Guide

## 🛠️ Installation Steps

### 1. Extract Project Files

unzip mcqproject.zip
```
cd mcqproject
```
## 2. Activate Virtual Environment
bash
### Windows:
```
cd myenv\Scripts\
activate

```

### Mac/Linux:
```
source myenv/bin/activate
```

## 3. Get Gemini API Key
Visit Google AI Studio

```
https://aistudio.google.com/app/apikey
```
Click "Create API Key"

Copy your key (starts with AIzaSy...)

## 4. Configure API Key
   
Open mcqapp/views.py in VS Code

Find line ~495 (search for GOOGLE_API_KEY)

Replace with your key:

python
os.environ["GOOGLE_API_KEY"] = "your_api_key_here"  # ← Paste your key

## 5. Install Requirements

```
cd mcqproject
```
```
pip install -r requirements.txt
```
```
pip install social-auth-app-django
```

## 6. Run Development Server

```
python manage.py runserver
```

Access at: http://127.0.0.1:8000

## 🔧 Troubleshooting

If Installation Fails:

# 1. Delete and recreate environment

```
deactivate
```
```
rm -rf myenv  # or `rmdir /s /q myenv` on Windows
or
Remove-Item -Recurse -Force myevn


```

# 2. Create fresh environment
```
python -m venv myenv
```
```
myenv\Scripts\
activate  # Reactivate

```

# 3. Install critical packages first

```
pip install social-auth-app-django
```
```
pip install -r requirements.txt
```

Missing Dependencies:

```
pip install --upgrade pip setuptools wheel
```
📂 Project Structure
text
mcq-project/
├── myenv/           # Python virtual environment
├── mcqproject/      # Django project
│   ├── mcqapp/      # Main application
│   │   └── views.py # Contains API configuration
│   └── manage.py    # Django management script
└── requirements.txt # Dependencies







# soi batch2 readme 
## all the eginnering 
*italic*
**bold**
#### Footnote12[^2]
***bold-italic***

~~strickthrough~~

### ordered list (1,2,3..)
1. first line
2. second line
3. third line

#### unorder list (-,+)
- first line 
+ second line 
- thrid line 

> Black Quote(highlet mark)

`for single line code ` 

**for mutiple line of code**
```
#include<stdio.h>
int main(){
int a,b;
printf("enter value");
scanf("%d,%d",&a,&b);
}
```

##### horizontal line(3--- or more that 3 ------)
-------------
###### insert any url

[my](https://www.google.com/)



###### insert any image 

![image](https://images.pexels.com/photos/674010/pexels-photo-674010.jpeg?_gl=1*muoa7a*_ga*NjkyMDgxOTgwLjE3NDk2MzY0NzY.*_ga_8JE65Q40S6*czE3NDk2MzY0NzUkbzEkZzAkdDE3NDk2MzY0NzUkajYwJGwwJGgw)

#### check list

- [x] aws
- [x] linux
- [ ] git
- [ ] devops


#### Footnote[^1]

[^1]:footnote

[^2]:footnote12


|name|college|District|
|----|---|---|
|bhuvana|abc|dfg|

