```python
# -*- coding: utf-8 -*-

class Researcher:
    def __init__(self):
        self.name = "Luu Minh Sao Khue"
        self.role = "PhD Student & AI Researcher"
        self.affiliation = (
            "Department of Mathematics and Mechanics, "
            "and Artificial Intelligence Research Center, "
            "Novosibirsk State University"
        )
        self.focus = [
            "Medical Image Analysis",
            "Self-Supervised Learning",
            "Multimodal Fusion",
            "AI Agents"
        ]
        self.projects = {
            "BrainFM": "Foundation model for multimodal brain MRI",
            "SatMFM": "Foundation model for multimodal satellite data",
            "ToolBrain": "Reinforcement learning framework for AI agents"
        }
        self.contact = {
            "Website": "https://luumsk.github.io",
            "LinkedIn": "https://linkedin.com/in/lmsk",
            "ResearchGate": "https://www.researchgate.net/profile/Minh-Sao-Khue-Luu"
        }

    def __repr__(self):
        return (
            f"<{self.role} | Exploring {', '.join(self.focus[:3])}, "
            f"and {self.focus[-1]}>"
        )


if __name__ == "__main__":
    me = Researcher()
    print(me)
```
