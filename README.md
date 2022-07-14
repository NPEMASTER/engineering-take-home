# Intro
In creating this project we strived to be both thorough in our assessment while remaining considerate of your time. Our intention was to make a project that is engaging to work on from a renewable energy perspective.

During the final technical interview this project will be the basis from which we discuss bigger concepts about coding philosophy. 

Thank you for taking the time to work on the RenewaFi take home assessment. 

# Time
In our understanding of this project four hours is enough time to complete the requirements. If you have not completed the project after four hours either stop and we will evaluate your work based on how far you got or continue and let us know how long it actually took.

If four hours is not enough time for you to finish the project, please do not feel obligated to continue working. A half-finished project with a clear explanation for how your time was spent is completely sufficient. 

# Process
 1. Clone this repository and commit your work to it.
 2. Work on the project (feel free to email us with any questions)
 3. Submit your project by emailing a .zip to **daniel@renewafi.com**
 4. Schedule a follow up interview (if not already scheduled)
 

# Evaluation
Aim for basics; skip the sticky parts. You are not being evaluated on the number of lines of code you write, but on the quality and economy of what you write to satisfy the challenge.

Key criteria:
 * Code completeness
 * Style
 * Economy
 * It runs!

When you submit your project we will review and schedule a 60-minute call to go over your work. On that call, be prepared to talk about
 * Design decisions
 * Trade-offs
 * Possible places to expand
 * Cool things you're proud of

# Background information

One of the core characteristics of a renewable energy power plants is that the electricity they delivery is intermittent; they will produce more or less megawatt hours depending on the time of year and time of day. Because a Power Purchase Agreement is a contract for electricity at a fixed price, the time and quantity of the delivery becomes very important in determining the potential profit or loss to a buyer; if the market price is higher than the PPA price then buyer will profit, if the market price is much lower than the PPA price then buyer will have a loss.

We understand the quantity of electricity a power plant will delivery with a table called a 12x24. This table has columns for each hour of the day (24) and rows for each month of the year (12). The individual cells of the table are the electricity that will be produced during that hour period of each month; the top left box is the amount of electricity delivered between 12:00am and 1:00am for each day in January.

We can calculate profit or loss of a deal by looking at the hourly pricing data posted by an ISO. 

# The Assignment

Imagine you are considering making a bid for to buy electricity from a power plant called Fun in Sun. The developer of that power plant will be delivery the electricity the Houston hub and will be doing so with the quantities in the attached 12x24 generation profile. Your company wants to know what the profit or loss of bid would have been using historical data. 

To do that you will need to build an app that takes a user's price input and calculates the profit or loss of a deal during the 2021 at the HB_HOUSTON settlement point. The app will need to use the `generationProfile.csv` included here combined with historical pricing data found here.

https://www.ercot.com/mp/data-products/data-product-details?id=NP4-180-ER

## Tasks
 - Import historical data for the year 2021 at HB_HOUSTON settlement point 
 - Take a user’s input for PPA price as input on the front end
 - Write an algorithm that sums the profit or loss for each hour in the year 2021. This will involve combing the following:
    - MWH price for each hours in the year (FYI there are 8760 hours in a year)
    - The quantity of MWHs the 12x24 says will be delivered in that hour
    - The users price

## Frontend
Your frontend end would ideally be a Typescript React app, though if another technology is much easier for you then go for that. The command to start this frontend should be included in a separate `README-your-name.md` file. Place your frontend code in `/frontend`.

## Backend
Your backend must be a Python app, though the web app should be whatever you think makes most sense for this project. The command to start this backend should be included in a separate ` README-your-name.md` file. Place your backend code in `/backend`.

