# Fortune Cookies
SPA Application with AJAX, jQuery, Handlebars, Sammy.js and System.js
Node.js and Express for the back-end

## Application description

The application provide the following functionality

* **Users** can **Register**, **Login** and **Logout** in the application
	* _Users provide `username`  and `password`_
* **Logged-in users** can:
	* **Share** a new fortune cookie
		* Providing `text` and `category`
	* **Re-share** an existing fortune cookie
		* This can be either:
			* A fortune cookie, shared by this user
			* A fortune cookie, shared by other user
	* **Like** or **dislike** a fortune cookie
	* **Get** their hourly fortune cookie
		* A random cookie from all shared cookies
		* This cookie is changed every hour
			* i.e. if the user asks for their fortune cookie at 11:30 and then again at 11:45, their fortune cookie will be the same
			* or if the user asks for their fortune cookie at 11:30 and then again at 12:00, the two fortune cookies may be different
				* It depends on the total count of fortune cookies
* **All users** (even not logged in) can **see** fortune cookies, that are shared by any user
* **Cookies** can be:
	* Sorted by `likes` or `shareDate`
	* Filtered by a single `category`
		* i.e. show only the fortune cookies in a given `category`

