# [rsschool-cv](https://rs.school/)

# Yauhen Ranko

## My contact info

* 🏠**Adress:** Uruchcha st. Minsk, Belarus
* ☎️**Phone:** +375 33 385 58 57
* 📧**Email:** yauhenranko@gmail.com
* **Telegram:** YauhenRanko  
[![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/in/yauhen-ranko-63a7801a3/)  
[![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/YauhenRanko)

## Summary

Currently I work as a FinTech Product Manager. My main goal is to learn how to create modern and user-friendly interfaces and, of course, learn how to do it correctly. I have a good understanding of business requirements and can convey these requirements to the development team. I like to understand problems in detail and solve them.

## Hard Skills:
1. Web programming in Python (Flask, FastAPI frameworks) - Basic knowledge
2. Working with relational and non-relational databases (PostgreSQL, SQLite, MongoDB)
3. Data Analytics (Excel, NumPy, Pandas, Matplotlib, BI)
4. UX/UI - Miro, Figma
 
## Soft Skills:
1. Work with a team - hiring, adaptation of employees, work with burnout and employee resource, optimization of tasks
2. Leadership - team motivation and overall commitment to the mission
3. Communication with external and internal customers
4. Work in multitasking mode

## Code example 🐍
```python
#part of the telegram bot code for selecting the required company
#analogue of yellow pages

#import necessary library and modules
from db import db, create_or_get_user, update_role
from utils import (city_keyboard, like_for_company, if_vote, skip_keyboard, 
                   start_keyboard, pagination_keyboard, count_company_keyboard,
                   pagination_keyboard_without_next, pagination_keyboard_without_previous, 
                   keyboard_for_first_text)

from telegram import ParseMode
from telegram.ext import ConversationHandler
from emoji import emojize

#function for validation users
def start_if_user(update, context):

    #request to a function to create or have a user
    #if the user is not found, then it is created and written to the DB
    user = create_or_get_user(db, update.effective_user, update.message.chat.id)
    user_data = 'user'
    update_role(db, user['user_id'], user_data)

    #show the user a new message
    update.message.reply_text(
        'Great, in which city are you looking for a company? ' + emojize(':office:', use_aliases=True),
        reply_markup = city_keyboard()
        )
    return 'service'
```  


## Education
1. Belarusian State University - Economy; commodity science
2. Learn Python 
3. Product University 


## Experience 
* Sales 
* Business Analysis
* Product Management


## Languages
1. English StreamLine Language School English sertificate Pre-Intermediate
2. Russian
