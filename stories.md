## interactive story 1
* greet
    - utter_greet
* restaurant_search{"location": "Bangalore"}
    - slot{"location": "Bangalore"}
    - action_check_location
    - slot{"location_flag": true}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_check_cuisine
    - slot{"cuisine_flag": true}
    - utter_ask_budget
* tell_budget{"budget": "low"}
    - slot{"budget": "low"}
    - action_search_restaurants
    - slot{"location": "Bangalore"}
    - slot{"restaurant_found_flag": false}

## interactive story 2
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "Bangalore"}
    - slot{"location": "Bangalore"}
    - action_check_location
    - slot{"location_flag": true}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_check_cuisine
    - slot{"cuisine_flag": true}
    - utter_ask_budget
* tell_budget{"budget": "medium"}
    - slot{"budget": "medium"}
    - action_search_restaurants
    - slot{"location": "Bangalore"}
    - slot{"restaurant_found_flag": true}
* affirm
    - utter_ask_email
* send_email{"email": "arish813@gmail.com"}
    - slot{"email": "arish813@gmail.com"}
    - action_send_email
    - slot{"email_sent_flag": true}
    - utter_email_sent
    - action_restart

## interactive story 3
* greet
    - utter_greet
* restaurant_search{"location": "Rishikesh"}
    - slot{"location": "Rishikesh"}
    - action_check_location
    - slot{"location": null}
    - slot{"location_flag": false}
    - utter_ask_location_again
* restaurant_search{"location": "Allahabad"}
    - slot{"location": "Allahabad"}
    - action_check_location
    - slot{"location_flag": true}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_check_cuisine
    - slot{"cuisine_flag": true}
    - utter_ask_budget
* tell_budget{"budget": "high"}
    - slot{"budget": "high"}
    - action_search_restaurants
    - slot{"location": "Allahabad"}
    - slot{"restaurant_found_flag": true}
* send_email{"email": "arish813@gmail.com"}
    - slot{"email": "arish813@gmail.com"}
    - action_send_email
    - slot{"email_sent_flag": true}
    - utter_email_sent
    - action_restart

## interactive story 4
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "mubaim"}
    - slot{"location": "mubaim"}
    - action_check_location
    - slot{"location": null}
    - slot{"location_flag": false}
    - utter_ask_location_again
* restaurant_search{"location": "Mumbai"}
    - slot{"location": "Mumbai"}
    - action_check_location
    - slot{"location_flag": true}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - action_check_cuisine
    - slot{"cuisine_flag": true}
    - utter_ask_budget
* tell_budget{"budget": "high"}
    - slot{"budget": "high"}
    - action_search_restaurants
    - slot{"location": "Mumbai"}
    - slot{"restaurant_found_flag": true}
* affirm
    - utter_ask_email
* send_email{"email": "arishnidaali@gmail.com"}
    - slot{"email": "arishnidaali@gmail.com"}
    - action_send_email
    - slot{"email_sent_flag": true}
    - utter_email_sent
    - action_restart

## interactive story 5
* greet
    - utter_greet
* restaurant_search{"cuisine": "chinese", "location": "Chandigarh"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "Chandigarh"}
    - action_check_location
    - slot{"location_flag": true}
    - action_check_cuisine
    - slot{"cuisine_flag": true}
    - utter_ask_budget
* tell_budget{"budget": "low"}
    - slot{"budget": "low"}
    - action_search_restaurants
    - slot{"location": "Chandigarh"}
    - slot{"restaurant_found_flag": true}
* deny
    - utter_goodbye
    - action_restart

## interactive story 6
* greet
    - utter_greet
* restaurant_search{"location": "Rishikesh"}
    - slot{"location": "Rishikesh"}
    - action_check_location
    - slot{"location": null}
    - utter_ask_location_again
* restaurant_search{"location": "Allahabad"}
    - slot{"location": "Allahabad"}
    - action_check_location
    - slot{"location_flag": true}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - action_check_cuisine
    - slot{"cuisine_flag": true}
    - utter_ask_budget
* tell_budget{"budget": "high"}
    - slot{"budget": "high"}
    - action_search_restaurants
    - slot{"location": "Allahabad"}
    - slot{"restaurant_found_flag": true}
* send_email{"email": "arish813@gmail.com"}
    - slot{"email": "arish813@gmail.com"}
    - action_send_email
    - slot{"email_sent_flag": true}
    - utter_email_sent
    - action_restart

## interactive story 7
* greet
    - utter_greet
* restaurant_search{"cuisine": "chinese", "location": "New Delhi"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "New Delhi"}
    - action_check_location
    - slot{"location_flag": true}
    - action_check_cuisine
    - slot{"cuisine_flag": true}
    - utter_ask_budget
* tell_budget{"budget": "high"}
    - slot{"budget": "high"}
    - action_search_restaurants
    - slot{"location": "New Delhi"}
    - slot{"restaurant_found_flag": true}
* deny
    - utter_goodbye
    - action_restart

## interactive story 8
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "channi"}
    - slot{"location": "channi"}
    - action_check_location
    - slot{"location": null}
    - utter_ask_location_again
* restaurant_search{"location": "Chennai"}
    - slot{"location": "Chennai"}
    - action_check_location
    - slot{"location_flag": true}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "American"}
    - slot{"cuisine": "American"}
    - action_check_cuisine
    - slot{"cuisine_flag": true}
    - utter_ask_budget
* tell_budget{"budget": "high"}
    - slot{"budget": "high"}
    - action_search_restaurants
    - slot{"location": "Chennai"}
    - slot{"restaurant_found_flag": true}
* affirm
    - utter_ask_email
* send_email{"email": "rsharath2204@gmail.com"}
    - slot{"email": "rsharath2204@gmail.com"}
    - action_send_email
    - slot{"email_sent_flag": true}
    - utter_email_sent
    - action_restart

## interactive story 9
* greet
    - utter_greet
* restaurant_search{"location": "jharkhand"}
    - slot{"location": "jharkhand"}
    - action_check_location
    - slot{"location": null}
    - utter_ask_location_again
* restaurant_search{"location": "Bhopal"}
    - slot{"location": "Bhopal"}
    - action_check_location
    - slot{"location_flag": true}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "Italian"}
    - slot{"cuisine": "Italian"}
    - action_check_cuisine
    - slot{"cuisine_flag": true}
    - utter_ask_budget
* tell_budget{"budget": "medium"}
    - slot{"budget": "medium"}
    - action_search_restaurants
    - slot{"location": "Bhopal"}
    - slot{"restaurant_found_flag": true}
* send_email{"email": "rsharath2204@gmail.com"}
    - slot{"email": "rsharath2204@gmail.com"}
    - action_send_email
    - slot{"email_sent_flag": true}
    - utter_email_sent
    - action_restart

## interactive story 10
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "Indore"}
    - slot{"location": "Indore"}
    - action_check_location
    - slot{"location_flag": true}
    - utter_ask_cuisine
* restaurant_search{"cuisine": "suth indian"}
    - slot{"cuisine": "suth indian"}
    - action_check_cuisine
    - slot{"cuisine": null}
    - slot{"cuisine_flag": false}
    - utter_ask_cuisine_again
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - utter_ask_budget
* tell_budget{"budget": "medium"}
    - slot{"budget": "medium"}
    - action_search_restaurants
    - slot{"location": "Indore"}
    - slot{"restaurant_found_flag": true}
* deny
    - utter_goodbye
    - action_restart

## interactive story 11
* restaurant_search{"cuisine": "spicy", "location": "New Delhi"}
    - slot{"cuisine": "spicy"}
    - slot{"location": "New Delhi"}
    - action_check_location
    - slot{"location_flag": true}
    - action_check_cuisine
    - slot{"cuisine": null}
    - slot{"cuisine_flag": false}
    - utter_ask_cuisine_again
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - utter_ask_budget
* tell_budget{"budget": "low"}
    - slot{"budget": "low"}
    - action_search_restaurants
    - slot{"location": "New Delhi"}
    - slot{"restaurant_found_flag": true}
* affirm
    - utter_ask_email
* send_email{"email": "arish813@gmail.com"}
    - slot{"email": "arish813@gmail.com"}
    - action_send_email
    - slot{"email_sent_flag": true}
    - utter_email_sent
    - action_restart
