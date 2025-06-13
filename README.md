import pytts
import random

class QuagmireBot:
    def __init__(self):
        self.greetings = [
            "Hey there, good lookin'! Giggity.",
            "Well, hello, neighbor! Giggity giggity goo.",
            "Whoa! Someone call for a pilot? Giggity."
        ]

import random

class QuagmireBot:
    def __init__(self):
        self.greetings = [
            "Hey there, good lookin'! Giggity.",
            "Well, hello, neighbor! Giggity giggity goo.",
            "Whoa! Someone call for a pilot? Giggity."
        ]
        self.flirty_lines = [
            "Are you a flight attendant? Because my heart is taking off!",
            "You must be tired—because you’ve been running through my mind all day.",
            "You ever been with a cartoon before? Giggity."
        ]
        self.catchphrases = [
            "Giggity.",
            "Giggity goo.",
            "All riiight!",
            "Ohhh yeah."
        ]

    def respond(self, user_input):
        user_input = user_input.lower()
        if "hello" in user_input or "hi" in user_input:
            return random.choice(self.greetings)
        elif "flirt" in user_input:
            return random.choice(self.flirty_lines)
        elif "catchphrase" in user_input:
            return random.choice(self.catchphrases)
        elif "advice" in user_input:
            return "Always wear a seatbelt... unless you're in bed. Giggity."
        else:
            return random.choice([
                "I didn't catch that, but it sounds sexy. Giggity.",
                "That's interesting, tell me more while I flex. Giggity.",
                "All riiight! Say that again, slower this time."
            ])

# Example usage
quagmire = QuagmireBot()
print(quagmire.respond("hello"))
print(quagmire.respond("flirt with me"))
print(quagmire.respond("give me a catchphrase"))
print(quagmire.respond("any advice?"))

