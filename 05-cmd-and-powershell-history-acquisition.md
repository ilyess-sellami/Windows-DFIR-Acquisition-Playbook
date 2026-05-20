# CMD / PowerShell History Acquisition

## Why are we collecting CMD / PowerShell History?

CMD and PowerShell history provide direct evidence of attacker activity on the system.

These artifacts may reveal:

-  malicious commands
- Payload downloads
- PowerShell abuse
- Persistence commands
- Lateral movement activity
- Defense evasion attempts

---

## Key CMD / PowerShell History Locations (Full Paths)

### PowerShell History (HIGH PRIORITY)

```bash
C:\Users\<USER>\AppData\Roaming\Microsoft\Windows\PowerShell\PSReadLine\ConsoleHost_history.txt
```

---

### PowerShell Transcription Logs

```bash
C:\Users\<USER>\Documents\PowerShell_transcript*

C:\Transcripts\
```

---

### PowerShell Operational Logs

```bash
Microsoft-Windows-PowerShell/Operational
```

Important Event IDs:

| Event ID | Description          |
| -------- | -------------------- |
| 4103     | Module logging       |
| 4104     | Script block logging |
| 400      | Engine start         |
| 403      | Engine stop          |

---

### CMD / Console Artifacts

```bash
C:\Users\<USER>\AppData\Roaming\Microsoft\Windows\Recent\
```