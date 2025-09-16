# Discord-Clone
<!-- TABLE OF CONTENTS -->

<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#1 Introduction">Introduction</a>
    </li>
    <li>
      <a href="#2 Key Features">Key Features</a>
    </li>
    <li>
      <a href="#3 Tech Stacks">Tech Stacks</a>
    </li>
    <li>
      <a href="#4 How to set up?">How to set up?</a>
    </li>
    <li>
      <a href="#5 Snaps">Snaps</a>
    </li>
  </ol>
</details>

# <a name="1 Introduction">Introduction:</a>

A clone of Discord with features like realtime chat app, roles, file sharing, servers...etc,
- React is used along with Redux to power front-end.
- Redux to manage state along with Redux Saga.
- React Routing with Error handling and Discord Loading between pages.
- Firebase is used for authentication and firestore to store messages, users and servers.
- Material UI is used along with SASS with a little of styled components for UI.

# <a name="2 Key Features">Key Features:</a>

- Server Channels
  
  i)   Create channels
  
  ii)  Delete channels
  
- Message Management

  i) Server owners can delete any message
  
  ii) Message author can delete and edit their own messages
  
- Member Management
  
  i) Kick members as the server owner
  
  ii) Easily leave the server by right clicking the server
  
  iii) Join servers with an invite code
  
- Server Management
  
  i) Create servers as you would in Discord

  ii) Edit server name, and icon URL in the server settings

  iii) Delete your server in the server settings
  
- User Management
  
  i) Manage your account by clicking the settings icon
  
  ii) Change your username, and avatar
  
  iii)Delete your user and prevent it from being used to login

# <a name="3 Tech Stacks">Tech Stacks:</a>

- TypeScript: 97.9%

- Javascript: 1.3%

- CSS: 0.8%

# <a name="4 How to set up?">How to set up?</a>

1. Clone the repository: git clone

   ```sh
   git clone https://github.com/<github_username>/Discord-Clone
   ```

2. Go to the Discord-Clone directory:

   ```sh
   cd discord-clone
   ```

3. To install the dependencies, run:

   ```sh
   npm install
   ```

4. To start the development server, run in terminal:

   ```sh
   npm run dev
   ```

Note : The project's backend is based on nodejs, so make sure you have node version 20 or above installed in your machine, if not refer to this: https://nodejs.org/en/download.

# Setup environment variables

## Supabase setup:

### 1. Project API setup

1. Go to [Supabase Dashboard](https://supabase.com/dashboard/projects) (create your account if you have not).
2. Create a new project.  
   ![Screenshot 2024-05-12 122005](https://github.com/meAyushSharma/file-converter--md-html/assets/146171218/b2332b87-9014-444e-847e-0edddfd41508)
3. Get your project url and anon api key.  
   Note : You should not reveal this api key as this works as a bridge between your database and project.
4. In your forked repo create a `.env.local` file, copy the contents from `.env.local.example` and paste the credentials in it:
   ```sh
   NEXT_PUBLIC_SUPABASE_URL=https(:)//some-string-here.supabase.co
   NEXT_PUBLIC_SUPABASE_ANON_KEY=anon-api-key-here
   ```
5. Setup your tables. Refer to [Table Setup Documentation](./table-setup.md)

Supabase is an open source firebase alternative, that provides Postgres database, Authentication, instant APIs, Edge Functions, Realtime subscriptions, Storage, and Vector embeddings.  
Refer to this [Documentation](https://supabase.com/docs), for more information.
