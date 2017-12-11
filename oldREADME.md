# onionup
## Uptime Checking Service for Tor Hidden Services

## Development Notes
Run vue webpacker in background: 

`bin/webpack-dev-server`


## This Weekend 

**Reid**

- [ ] Vue tutorial/toyapp in vue
- [ ] Build frontend API for user auth 

**Jay**

- [ ] Vue tutorial/toyapp in vue
- [ ] Install Tor
- [ ] Modals (login), layout

**Chris** 

- [ ] Vue tutorial/toyapp in vue
- [ ] AWS & Tor Client testing/scripting (Proof of concept for live version with traffic)

**Artem**

- [ ] Vue tutorial/toyapp in vue
- [ ] Install Tor
- [ ] Workers (sidekiq) concurrent processes, gathering ping information, load time, component interactions on hidden services (stretch)

## Monday

**Reid**

- [ ] Site show page 
- [ ] User show page
- [ ] Settings show page 

**Jay**

- [ ] Index Component 
- [ ] Sidebar/page styling, navigation

**Chris** 
- [ ] Have rails server running concurrently with onion proxy able to make ping requests
- [ ] Bootup tor and rails with one command 

**Artem**

- [ ] Making APIs for frontend to get information 
- [ ] Timestamped data for graphs

## Tuesday

**Reid**

- [ ] Graphing ping data in d3

**Jay**

- [ ] Create site card component for index 

**Chris** 

- [ ] Store ping data in database and requesting data 

**Artem**

- [ ] Look into websockets (Application Cable) connecting front and backend

## Wednesday

**Reid**

- [ ] Display historical data from backend to frontend

**Jay**

- [ ] 

**Chris** 

- [ ] Display historical data from backend to frontend 

**Artem**

- [ ]

## Thursday

**Reid**

- [ ] 

**Jay**

- [ ] 

**Chris** 

- [ ] 

**Artem**

- [ ]

## Friday

**Reid**

- [ ] 

**Jay**

- [ ] 

**Chris** 

- [ ] 

**Artem**

- [ ]


### Project Description

Pingdom inspired Tor uptime checker that displays the health of hidden services and clearnet websites

User authentication
* Username (null: false)
* Password (null: false)
* Optional email
* Modal popup
* Recover account with email
* Devise gem
* Explanation of why we chose devise encryption (how it adds to functionality)

User Settings
* Change password
* Add or edit email
* Autogenerated Profile picture

View index of saved URLs. Each site card has
* Health (up or down)
* Ping Time
* Live graph (d3)
* URL
* Add new site button
* Tab different windows of time e.g., seconds, minutes, days, months
* Render time?

New URL
* Allow ip address
* Allow any format of URL

Site show page
* Delete button
* Larger graph
* Edit alias (customize)
* Edit description
* ip address
* Download PDF?
* Download CSV?

Settings section?
* Change color scheme?
* Edit units (e.g. ms vs s)?


Stretch Goals
* Ping sites even while offline and store information in DB
* Fullscreen or presentation dev mode 


### Technologies
* Ruby on Rails
* VueJS
* D3 for graphs
* Tor
* Sidekiq
* Devise

Stretch Goals
* Ping sites even while offline and store information in DB
* Fullscreen or presentation dev mode

Health: How long site is up vs how long site is down
Pingtime: Ping response time
Successful load/loadtime
Click component on page


### TO DO:

* Wireframe the different components
* Plan frontend/backend routes
* Users should be allowed to log in with JUST a username, optionally an email as well
* Ping sites on user's account at a fixed interval (e.g. every 5 seconds)
* Run tor from the server
* Distinguish between a downed website/service and our server being down
* Live graph on sites page
* Vue frontend to make single page app
* Ping from multiple locations?
* SMS option?
* Email when sites are down?

## Development

## Feature Branch Workflow - Steps to take if you want to add a feature
1. Navigate to master branch and pull the latest code.
2. Create a new brach off of master. Name it as the feature you are implementing.
3. As you work on the feature, add and commit as you would normally.
4. Push you branch to your remote repo (Github) and push your changes every so often. (Do not merge to master yet)
5. If there are issues with your commits as you are working on your feature, teammates can comment on these commits and help you with your feature (check the branch out themselves if need be).
6. Upon feature completion, create a Pull Request on Github, after this is approved by teammates the feature branch is merged into master.


### For local development:

1. run tor from terminal
2. rails s
3. open localhost:3000 in browser

## Backup ideas

* Onion site crawler
* Peer to peer distributed pingdom clone  