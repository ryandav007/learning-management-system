## LMS Platform

## Development Status

- Versions and dependencies have been updated.
- Comments have been added and code has been tidied up.
- Occasional reports of black screen or other issues at runtime have been received, possibly related to Clerk integration.

**Key Features:**

- Browse and filter courses
- Purchase courses using Stripe
- Mark chapters as completed or uncompleted
- Progress calculation of each course
- Student dashboard
- Teacher mode
- Create new courses
- Create new chapters
- Easily reorder chapter position with drag and drop
- Upload thumbnails, attachments, and videos using UploadThing
- Video processing using Mux
- HLS Video player using Mux
- Rich text editor for chapter description
- Authentication using Clerk
- ORM using Prisma
- MySQL database using Planetscale

**Enhancements:**

- Added a search function to the courses page
- Improved the user interface of the student and teacher dashboards

**Planned Enhancement:**
Integrate Elliot Chong's Quizmify into this.

**Usage:**

To use this repository, you will need to have Node.js and NPM installed on your machine. Once you have installed the necessary dependencies, you can clone the repository and run the following commands:

**Deployment:**

To deploy the application to production, you will need to sign up for accounts on the following services:

Vercel https://vercel.com - for server-less hosting.

Mux https://mux.com - for Videos storage.

Clerk https://clerk.com 

MongoDB Atlas https://mongodb.com 

UploadThing https://uploadthing.com/ for serverless upload storage.

Stripe Payments: https://stripe.com


To reset the database, run

    npx prisma migrate reset
    npx prisma db push


Note also if reinitializing the datbase you also need to run:
node scripts/seed.ts
