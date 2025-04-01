# Check if the log file exists, if not create it
if [ ! -f "$MOUNT_DIR/filebrowser.log" ]; then
    echo "Log file not found, creating it..."
    sudo touch "$MOUNT_DIR/filebrowser.log"
    sudo chown $USER:$USER "$MOUNT_DIR/filebrowser.log"
    echo "Log file created at $MOUNT_DIR/filebrowser.log"
fi
