
```javascript

mermaid.ganttConfig = { titleTopMargin: 25, barHeight: 20, barGap: 4, topPadding: 75, sidePadding: 75, };


```


```mermaid

gantt

	title Individual Project timeline
	dateFormat DD-MM-YYYY
	
	section Design
	Get test data:ade1, 17-11-2023, 12d
	
	section Development
	Sprint 1: imp1, 29-01-2024, 14d
	Sprint 2: imp2, after imp1 12-02-2024, 14d
	Sprint 3: imp3, after imp2 26-02-2024, 14d
	Sprint 4: imp4, after imp3 11-03-2024, 14d
	
	section Report
	Write up report: rep1, 22-04-2024, 21d

```


