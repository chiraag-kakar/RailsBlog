# RailsBlog
A Blogging platform built using Ruby on Rails with the help of Paiza Cloud IDE

## Inroduction to the Platform :
* The RailsBlog is built upon the [Paiza Cloud Platform](https://paiza.cloud/en/).
* Sign up for the mentioned cloud service.
* On the free plan we can use the server / container (we will be creating) for 24 hours after which the server will be restored.
* Also the server gets suspended after 240 minutes of usuage.
* So the free plan is more than enough if we can patiently built the project within the stipulated period.

## Alternative Platforms :
* *AWS Cloud9* is another popular cloud-based **Integrated Development Environment (IDE)**

# Let's get started :

## Create a Blank Rails App -
* After signing up to the cloud service with the credentials (mail or username and password) create a new server.
* Then go to the terminal and create a blank rails app using the following command :

```
rails new blog
```
'blog' will be the name of our application.

The dependencies will take some minutes to install.

## Changing the database engine's version to the required version - 
* Inside the main Rails folder "blog" , there will be "gemfile"
* Inside that file replace the following line :
```
gem 'sqlite3'
```
  with 

```
gem 'sqlite3', '1.3.13'
```

* Also make sure that the Autosave box is checked.

After making changes in the gemfile , enter the following commands in the terminal to update and install the specified version of dependencies :
```
cd blog
bundle install
bundle update
```

## Activating the Server :
The server can be activated by any one of the following commands :
```
rails server -b $IP -p $PORT
```
*or*

```
rails server
```
*or*

```
rails s
```

## Creating Blogposts
```
rails generate scaffold Post title:string body:text

```
Rails will create a bunch of folders with functionalities in the app directory.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
