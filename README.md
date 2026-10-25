
from dataclasses import dataclass, field


@dataclass
class Researcher:
    name: str = "Luu Minh Sao Khue"
    role: str = "PhD Candidate | AI Researcher"
    affiliation: str = (
        "The Artificial Intelligence Research Center, "
        "Novosibirsk State University"
    )

    research_interests: list[str] = field(default_factory=lambda: [
        "Multi-Agent Systems",
        "LLM Reasoning and Optimization",
        "AI Oversight and Reliability",
        "Self-Improving AI Systems",
        "Medical AI",
    ])

    research_projects: list[str] = field(default_factory=lambda: [
        "Optimization of multi-agent communication",
        "Budgeted oversight for reliable AI agents",
        "Capability-aware reasoning in vision-language models",
        "Representation learning for medical image analysis",
    ])

    publications: dict[str, str | int] = field(default_factory=lambda: {
        "Total": 13,
        "Q1 Journals": 2,
        "Q2 Journals": 1,
        "CORE A*/A Conferences": 2,
    })

    contact: dict[str, str] = field(default_factory=lambda: {
        "Website": "https://luumsk.github.io",
        "LinkedIn": "https://linkedin.com/in/lmsk",
        "ResearchGate": "https://www.researchgate.net/profile/Minh-Sao-Khue-Luu",
    })

    def __str__(self) -> str:
        return (
            f"{self.name} | {self.role}\n"
            "Building intelligent and reliable AI systems."
        )


if __name__ == "__main__":
    me = Researcher()
    print(me)
