# Quiz Application - JSON File Format

## Übersicht

Diese Quiz-Anwendung lädt Fragen dynamisch aus JSON-Dateien im aktuellen Verzeichnis. Sie können mehrere JSON-Dateien mit Fragen erstellen, und die Anwendung wird alle laden und mischen.

## Unterstützte JSON-Formate

### Format 1: Array von Fragen

```json
[
  {
    "question": "Ihre Frage hier?",
    "answers": ["Antwort A", "Antwort B", "Antwort C", "Antwort D"],
    "correct": 1,
    "explanation": "Erklärung der richtigen Antwort"
  }
]
```

### Format 2: Objekt mit Fragen-Array

```json
{
  "title": "Quiz Titel (optional)",
  "questions": [
    {
      "question": "Ihre Frage hier?",
      "answers": ["Antwort A", "Antwort B", "Antwort C", "Antwort D"],
      "correct": 0,
      "explanation": "Erklärung der richtigen Antwort"
    }
  ]
}
```

## Feld-Beschreibungen

- **question** (erforderlich): Der Fragetext
- **answers** (erforderlich): Array mit mindestens 2 Antwortmöglichkeiten
- **correct** (erforderlich): Index der richtigen Antwort (0-basiert)
- **explanation** (optional): Erklärung, die nach der Antwort angezeigt wird

## Dateinamen

Die Anwendung sucht automatisch nach JSON-Dateien. Empfohlene Namen:

- `questions.json`
- `quiz.json`
- `algorithmus-fragen.json`
- `fragen.json`

Sie können aber auch beliebige andere Namen mit `.json` Endung verwenden.

## Beispiele

Siehe die mitgelieferten Dateien:

- `sample-questions.json` - Einfaches Array-Format
- `datenstrukturen-quiz.json` - Objekt-Format mit Titel
