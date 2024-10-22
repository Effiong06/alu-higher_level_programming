#!/bin/bash

# Check if the PYFILE environment variable is set
if [ -z "$PYFILE" ]; then
  echo "Error: PYFILE environment variable is not set."
  exit 1
fi

# Check if the specified Python file exists
if [ ! -f "$PYFILE" ]; then
  echo "Error: File $PYFILE does not exist."
  exit 1
fi

# Run the Python script
python3 "$PYFILE"

# Check the exit status of the Python script
if [ $? -eq 0 ]; then
  echo "Script executed successfully."
else
  echo "Script execution failed."
fi
