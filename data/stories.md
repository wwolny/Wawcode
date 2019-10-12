## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## long_conv2
* greet
    - utter_greet
* mood_unhappy
    - utter_cheer_up
    - utter_did_that_help
* deny
    - utter_goodbye
* goodbye
    - utter_goodbye

## long_conv
* greet
    - utter_greet
* mood_great
    - utter_happy
* mood_question
    - utter_bot_happy
* mood_great
## check_p1
* greet
  - utter_greet
> check_asked_q

## check_p2a
> check_asked_q
* affirm
  - utter_happy
>check_bye

## check_p2b
> check_asked_q
* deny
  - utter_cheer_up
  - utter_did_that_help
>check_bye

## check_p3
>check_bye
* affirm OR deny OR mood_great
  - utter_goodbye

##check_p4
>check_bye
* mood_question
  - utter_happy
> check_bye

##check_p5
>check_bye
* q_rurobot
  - utter_iamrobot
>check_bye

## Generated Story -323373425631219000
* mood_unhappy
    - rewind
* affirm
    - rewind
* greet
    - utter_greet
* mood_great
    - utter_happy
* mood_great
    - rewind
* lost_info{"thing": "koszulkę"}
    - utter_qplace
* mood_great
    - rewind
* lost_place{"address": "ulicy Gocławskiej 304"}
    - utter_qphone
* mood_great
    - rewind
* lost_phone{"phone": "324234123"}
    - utter_qdescription
* mood_great
    - rewind
* lost_description{"description": "Zostawiłem go na ławce przy sklepie Carrefour"}
    - utter_qtime
* mood_great
    - rewind
* lost_time{"day": "wczoraj", "hour": "13"}
