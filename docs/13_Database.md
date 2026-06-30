# Base de datos

## users

id

username

password_hash

display_name

avatar

coins

gems

premium_until

language

theme

created_at

last_login

last_daily_reward

statistics_json

settings_json

---

## runs

id

user_id

region

current_zone

current_node

difficulty

gold

created_at

updated_at

finished

---

## run_pokemon

id

run_id

pokemon_id

nickname

level

hp

max_hp

status

experience

moves_json

held_item

relic

position

is_shiny

---

## run_inventory

id

run_id

item_id

quantity

---

## run_relics

id

run_id

relic_id

obtained_at

---

## run_events

id

run_id

event_id

choice

result

---

## achievements

id

name

description

icon

---

## user_achievements

user_id

achievement_id

obtained_at

---

## statistics

user_id

total_runs

wins

losses

captures

shinies

highest_level

best_time

favorite_pokemon
