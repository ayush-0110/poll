## Poll App using Spring Boot and ReactJS

## Steps to Setup the server:

1. **Clone the application**

	```bash
	git clone https://github.com/callicoder/spring-security-react-ant-design-polls-app.git
	cd polling-app-server
	```

2. **Create MySQL/PostgreSQL database**

3. **Configure MySQL/PostgreSQL username and password**

4. **Run the app**

	You can run the spring boot app by typing the following command -

	```bash
	mvn spring-boot:run
	```

	The server will start on port 5000. The spring boot app includes the front end build also, so you'll be able to access the complete application on `http://localhost:5000`.

5. **Add the default Roles**
	
	The spring boot app uses role based authorization powered by spring security. Please execute the following sql queries in the database to insert the `USER` and `ADMIN` roles.

	```sql
	INSERT INTO roles(name) VALUES('ROLE_USER');
	INSERT INTO roles(name) VALUES('ROLE_ADMIN');
	```

	Any new user who signs up to the app is assigned the `ROLE_USER` by default.

## Steps to Setup the Client:

Type the following command to install the frontend dependencies -

```bash
npm install
```

Then run this command to start the application:

```bash
npm start
```

The front-end server will start on port `3000`.
