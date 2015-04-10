# I want to start the installation on debian from scratch, how can I start over?

Start with a clean `node_modules/` folder:

    sudo rm -Rf node_modules/

Be sure everything in `~/.npm/` belongs to you:

    sudo chown $USER:$USER -Rf ~/.npm/

Now start with the paragraph "Installing dependencies" from the README.md


# Can I use the same `nodes.json` from the old ffmap-d3 project?

No, the meshviewer uses a completely reworked data structure. You need the latest ffmap-backend to generate the right data.