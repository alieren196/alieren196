<p align="center">
  <a href="https://github.com/alieren196">
    <img src="https://avatars.githubusercontent.com/u/81759021?v=4" alt="Avatar" width="260" height="260">
  </a>

  <h1 align="center">Ali Eren</h1>

  <p align="center">
      Hi there 👋 I’m currently working on the Python, WEB, Robotics and Blockchain.
    <br />
    <br />

  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=alieren196&theme=blue-green&layout=compact)](https://github.com/anuraghazra/github-readme-stats" alt="Most used languages">
  <br />
  <br />
  <img src="https://github-readme-stats.vercel.app/api?username=alieren196&theme=blue-green&show_icons=true)](https://github.com/anuraghazra/github-readme-stats" alt="Ali Eren's github stats">

  <br />
  <br />
  
  <img src="https://github-profile-trophy.vercel.app/?username=alieren196&theme=darkhub&row=1&no-bg=true)](https://github.com/ryo-ma/github-profile-trophy" alt="Ali Eren's github trophy">
  
  </p>
</p>

<p align="center">
  <img align="center" src="/github-metrics.svg" alt="Metrics" width="450">
</p>

```python
#!/usr/bin/python3
# -*- coding: utf-8 -*-


import json
from hashlib import sha256


class Ali_Eren_Tabak:
    """
    Ali Eren Tabak is a human, loves programming, at the same time ı am working Decentra Network
    """

    def __init__(self):
        self.type = "Human-Male"
        self.age = 18
        self.country = "Turkey"
        self.city = "Gaziantep"

        self.job = "Programmer"
        self.working_areas = [
            "Python",
            "WEB",
            "Blockhain"
        ]
        self.projects = [
            ["Decentra Network", "https://github.com/alieren196/Decentra-Network"],
            ["Jack_Assistant", "https://github.com/alieren196/Jack_Asisstant"],

        ]
        self.linkedin = "https://www.linkedin.com/in/ali-eren-tabak-48300320b/"
    def dump_json(self):
        """
        Returns a json containing the Ali_Eren_Tabak data.
        """

        data = {
            "type": self.type,
            "age": self.age,
            "country": self.country,
            "city": self.city
        }
        return data

    def get_hash(self, encoding="ascii"):
        """
        Returns a sha256 created using the dump_json() function.
        """

        transaction_data = json.dumps(self.dump_json()).encode(encoding)
        return sha256(transaction_data).hexdigest()        
        
if __name__ == "__main__":
    the_ali = Ali_Eren_Tabak
    print(f"ID: {the_ali.get_hash()}")

    print("\nProjects:")
    for project in the_ali.projects:
        print(f"{project[0]}: {project[1]}")

    print("\nLibraries:")
    for library in the_ali.libraries:
        print(f"{library[0]}: {library[1]}") 
        
    
    print(f"\nLinkedIn: {the_ali.linkedin}")

```        
        
