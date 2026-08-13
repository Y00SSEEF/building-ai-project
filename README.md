# Creator AI
Building AI course project

## Summary
Creator AI is a specialized assistant built to help YouTube creators turn raw video ideas into fully structured channel content. Instead of spending hours writing video scripts, crafting catchy title hooks, or drafting SEO descriptions, it converts rough notes and video outlines into YouTube-ready content.

## Background
Maintaining a successful YouTube channel requires consistent uploading, but scriptwriting and packaging long-form or short-form content can lead to creative burnout.

* **Scriptwriting bottlenecks:** Outlining long videos or pacing fast YouTube Shorts scripts from scratch takes up a huge chunk of time.
* **Repetitive tasks:** Writing engaging title hooks, timestamp breakdowns, and SEO-friendly video descriptions for every upload is tedious.
* **Personal motivation:** I wanted a dedicated tool to help YouTubers streamline their pre-production workflow so they can spend more time actually filming and editing.

## How is it used?
The tool is meant for YouTubers, video editors, and channel managers. It runs either as a web dashboard or a simple text-editor helper tool.

1. **Input:** You enter a topic idea, rough bullet points, or a quick voice note summary.
2. **Processing:** Creator AI generates a structured video script (with intro hooks and call-to-actions), catchy video titles, and an SEO description.
3. **Review:** You refine the script, adjust the tone to match your personal channel style, and proceed to filming.

## Data sources and AI methods

### Data Sources
* User-provided topic outlines, rough scripts, and video transcripts.
* Public YouTube metadata (e.g., search trends, video titles, and tag structures) for optimizing descriptions.

### AI Methods
* **Natural Language Processing (NLP):** Using language models for script generation, text summarization, and tone adaptation.
* **Prompt Engineering:** Custom templates designed to format output into clean YouTube script sections (Hooks, Intros, Main Points, and Outros).

```python
# Quick demo of generating YouTube video title hooks
def generate_youtube_hooks(topic, style="long_form"):
    if style == "short":
        return f"You won't believe what happens when you try {topic}!"
    else:
        return f"Why Everyone Is Talking About {topic} (And What You Need To Know)"

print(generate_youtube_hooks("AI Tools", "long_form"))
