# README

<<<<<<< HEAD
=======
This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

>>>>>>> 5732a9f1faa2338fcbc0a51892a595f14fdcb8bb
# chat-space DB設計
## usersテーブル
|Column|Type|Options|
|------|----|-------|
|email|string|null: false|
|password|string|null: false|
<<<<<<< HEAD
|name|string|null: false|
### Association
- has_many :messages
=======
|username|string|null: false|
### Association
- has_many :tweets
>>>>>>> 5732a9f1faa2338fcbc0a51892a595f14fdcb8bb
- has_many :groups_users
- has_many  :groups,  through:  :groups_users


<<<<<<< HEAD
## messagesテーブル
|Column|Type|Options|
|------|----|-------|
|image|text||
|text|text||
|user_id|integer|null: false, foreign_key: true|
### Association
- belongs_to :user
- belongs_to :group
=======
## tweetsテーブル
|Column|Type|Options|
|------|----|-------|
|text|text|null: false|
|image|string|null: false|
|user_id|integer|null: false, foreign_key: true|
### Association
- belongs_to :user
>>>>>>> 5732a9f1faa2338fcbc0a51892a595f14fdcb8bb

## groupsテーブル
|Column|Type|Options|
|------|----|-------|
<<<<<<< HEAD
|name|string|null: false|
### Association
- has_many :groups_users
- has_many :messages
=======
|groupname|string|null: false|
|chatmember|string|null: false|
### Association
- has_many :groups_users
>>>>>>> 5732a9f1faa2338fcbc0a51892a595f14fdcb8bb
- has_many  :users,  through:  :groups_users

## groups_usersテーブル
|Column|Type|Options|
|------|----|-------|
|user_id|integer|null: false, foreign_key: true|
|group_id|integer|null: false, foreign_key: true|
### Association
- belongs_to :group
- belongs_to :user
<<<<<<< HEAD
=======


>>>>>>> 5732a9f1faa2338fcbc0a51892a595f14fdcb8bb
