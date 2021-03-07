# Access a user's server

Accessing a user's server is very useful when trying to debug or reproduce an issue they might have. This facility is available to admins via the admin panel. 

1. You can access the admin panel by clicking the 'Admin' button in the top bar
   in your hub control panel.  Alternatively, you can go to this URL in our
   browser: `https://<your-hub-url>/hub/admin`.

2. You can click `access server` to gain control of a user's currently running server. If it isn't running, you can click `start server` first and wait for it to start.

   ```{figure} ../../images/access-server.png
   Clicking "access server" will allow you to control the user's session.
   ```

3. This will bring you to the default interface that the user would have seen if they had just logged into the hub. From here, you can navigate to the notebook the user has reported issues with, and help them debug.

   ```{warning}
   If you both work on the same notebook at the same time, you will just
   overwrite each other's code! The state of the notebook will be that of
   whoever saved the notebook last. There is no Google Docs' style
   real-time collaboration yet, although [it is coming](https://github.com/jupyterlab/rtc)
   ```

   ```{warning}
   When you control a user's server, all of your actions will be run *as
   if the user ran it themselves*. This can be confusing for some users
   and is generally not best-practice. We recommend telling users when
   you are taking over their session, and using this feature mostly to understand what the user was trying to do, rather than to make major
   changes to their code or notebook outputs.
    ```