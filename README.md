# jellyfin-actor-processor
This is a simple script that will refresh the actors from the Jellyfin API.
I made this to fix the issue where the actor's image are not showing up in the Jellyfin until you click the actor to view the actor's detail page or delete the actor image once.

# How to use
1. Clone this repository
2. Run `python main.py -url <Jellyfin URL> -key <Jellyfin API Key>`

# Example
`python main.py -url http://localhost:8096 -key 1234567890abcdef1234567890abcdef`
![image](https://github.com/user-attachments/assets/dd344991-a811-41cb-ae4d-79eba4c28a08)

# Options
```shell
$python .\main.py --help

usage: main.py [-h] -url URL -key API_KEY [-f] [-r RETRIES]

Jellyfin Actor Processor

options:
  -h, --help            show this help message and exit
  -url URL, --url URL   Jellyfin server URL
  -key API_KEY, --api-key API_KEY
                        Jellyfin API key
  -f, --force           Process all persons
  -r RETRIES, --retries RETRIES
                        Maximum number of retries for failed requests
```

# Screenshots
Before:
![9332cebedaf073e59e09bd739195351](https://github.com/user-attachments/assets/f2c9777c-0ba9-486d-af4e-4e4ef6f294f4)
![d5802d6ce8340f9aa0633ba243a18bb](https://github.com/user-attachments/assets/33cdd647-14d9-4652-98e4-1fe92eb92a89)
![6d22981ab0e7258f92ce4411df1db58](https://github.com/user-attachments/assets/227100bf-495d-4fc3-883f-cd218eb066d5)
After:
![image](https://github.com/user-attachments/assets/527400d0-12fb-4376-819f-802304912add)
![image](https://github.com/user-attachments/assets/32f30007-deb8-428b-99d8-cb06ea028894)
![image](https://github.com/user-attachments/assets/1c0778bf-f938-4d8a-9c5a-8418ad9a1532)
