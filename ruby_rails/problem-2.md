Problem 2
===
We are fetching free time slots of a user from two calendars (Google calendar & iCloud calendar). Both the service gives similar output as show below

Response from Google Calendar Service

```
[
	{
		start: "2015-11-01T10:00:00.00+08:00",
		end: "2015-11-01T11:00:00.00+08:00"
	},
	{
		start: "2015-11-01T11:00:00.00+08:00",
		end: "2015-11-01T14:00:00.00+08:00"
	},
	{
		start: "2015-11-01T15:00:00.00+08:00",
		end: "2015-11-01T17:00:00.00+08:00"
	}
]
```

Response from iCal Calendar Service

```
[
	{
		start: "2015-11-01T12:00:00.00+08:00",
		end: "2015-11-01T13:00:00.00+08:00"
	},
	{
		start: "2015-11-01T13:00:00.00+08:00",
		end: "2015-11-01T14:00:00.00+08:00"
	},
	{
		start: "2015-11-01T14:00:00.00+08:00",
		end: "2015-11-01T15:00:00.00+08:00"
	},
	{
		start: "2015-11-01T15:00:00.00+08:00",
		end: "2015-11-01T16:00:00.00+08:00"
	}
]
```

As you can see that time slot [11:00-14:00] from Google overlaps time slots [12:00-13:00] and [13:00-14:00] in the iCal response.

**Write a code in ruby that will**

1. take these two objects and output a unique free time slots (no duplicates and overlaps).
2. Order the union chronologically

##### Output

```
[
	{
		start: "2015-11-01T10:00:00.00+08:00",
		end: "2015-11-01T11:00:00.00+08:00"
	},
	{
		start: "2015-11-01T11:00:00.00+08:00",
		end: "2015-11-01T14:00:00.00+08:00"
	},
	{
		start: "2015-11-01T14:00:00.00+08:00",
		end: "2015-11-01T15:00:00.00+08:00"
	},
	{
		start: "2015-11-01T15:00:00.00+08:00",
		end: "2015-11-01T16:00:00.00+08:00"
	}
]
```
