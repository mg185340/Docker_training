Docker training under John Kerry. `Current Task:`

Create a dockerfile that produces a container such that:

- The container runs nginx 
- GZIP  compression is enabled for image datatypes
- The content returned when visiting http://localhost:80  (when the container port is mapped to local port 80)  is:
```
    <html>
        <h1>QA</h1>
    </html>

    <html>
        <h1>STAGING</h1>
    </html>

    <html>
        <h1>Prod</h1>
    </html>
```
respectively when a runtime environment variable NGINX_ENVIRONMENT is set to qa, staging, or prod as a part of the container runtime command (like the  ORRB example)