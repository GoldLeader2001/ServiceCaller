# [Service Caller](https://service-caller.web.app/)

# OVERVIEW

A web app that users can use to call local or popular businesses. This was built using a Java Spring Backend to act as an API that handled all of the connections to the call service and to the MongoDB database. The frontend is a React app built from the ground up using Material-UI v5 as the primary decorator. The actual calling is done using Twilio's API to create a call between the user's phone and the service's phone. The backend is deployed using GCP's Cloud Run service, the frontend is hosted by Firebase, and I am using MongoDB Atlas for my cloud database.

# HOW TO (User Side)

1. Navigate to [https://service-caller.web.app/](https://service-caller.web.app/) You will be brought to the landing page
2. Click the "Sign In" button, once on the sign in page you can enter the information (email: [guest@servicecaller.com](mailto:guest@servicecaller.com) and password: "password") to access the test account
3. If you want to test the calling feature you will need to add your phone number to the test account or create your own account*
4. From the home page, you can view your recent call history(placeholder), your balance(placeholder with minimal function), and your favorites list(works!)
5. On the top nav bar, you can go to the homepage by clicking the title of the site, or you can go to the contact page to view the site's contact information(not implemented), or you can go to the search page to find a business you may want to call, or you can go to your profile page
6. On the profile page, you can update your profile info and add an avatar to your profile
7. On the search page, you can type in the search bar and it will dynamically update the list of businesses(all of which are not real businesses of course) the search cards contain the business's rating and the total number of calls(neither are implemented) and if you select the "View" button you can navigate to their page.
8. From the business's page, you can make a reservation(partially implemented), add the business to your favorite list by clicking the heart icon, or you could of course click the "Call" button to initiate a call with the business.

*If you want to create your own account you would select the sign up option and then fill out the fields with whatever information you'd like, it doesn't have to be real info, to create a new profile (if you want the calling to work you would need to put your own phone number)

# HOW TO (Business Side)

1. If you wish to see what the business's side of the site looks like you can go to [https://service-caller.web.app/54676](https://service-caller.web.app/54676) and sign in with the email: [fakeemail@gmail.com](mailto:fakeemail@gmail.com) and password: "password"
2. You will be navigated to the home page for the "Andrew's Outdoor Emporium" business where you will be able to see any reservations users have made with this business by going through the days on the schedule card
3. You can also make the business "live" by clicking the "Make Available" button.
4. You will also be able to edit the business information as well
