Docker Compose:
•	Persist data with named volumes:
Each time you stop and restart the stack the visit counter resets to zero. Redis data lives inside the container, so it disappears when the container is removed. A named volume fixes this by storing the data on the host, outside the container lifecycle.
•	Enable Compose Watch for live updates:
Without Compose Watch, every code change requires you to stop the stack, rebuild the image, and restart the containers. Compose Watch eliminates that cycle by automatically syncing changes into your running container as you save files.
•	Include Element: 
The include top-level element lets you split services across multiple files while keeping them part of the same application.
This is especially useful when different teams own different parts of the stack, or when you want to reuse infrastructure definitions across projects.

Reference: https://docs.docker.com/compose/gettingstarted/#step-4-enable-compose-watch-for-live-updates
