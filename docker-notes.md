 Career guide

That's an excellent idea. Much more organized.

You're absolutely right. As you learn more technologies, keeping separate files for each one is a much cleaner and more professional way to structure your repository.

Let's do that instead.

Step 1: Create the New Docker Notes File

Make sure you are in your project directory:

cd ~/devops-cheatsheet

Now, run this command. It will create a brand new file called docker-notes.md and put our content inside it.
Bash

cat <<EOF > docker-notes.md
# Docker Learning Notes

## Phase 2: Running a Web Server

- **Image:** The blueprint or recipe (e.g., \`nginx\`).
- **Container:** A running instance of an image.
- **Port Mapping (\`--publish\`):** Connects a port on the host machine to a port inside the container so the outside world can access the service.

### Command to run an NGINX server:
\`\`\`bash
docker run --publish 8080:80 --detach --name my-web-server fnginx
\`\`\`
EOF
