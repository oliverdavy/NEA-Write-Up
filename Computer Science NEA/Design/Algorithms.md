%%
#Complete 
#Design
%%
# Algorithms

These are pseudo-code versions of algorithms that will be used to guide development. They will likely change to fit the framework being used, however their main purpose will remain.

## Metronome

```
function StartStop(bool currentState){
	newState = !currentState
	return newState
}
```

```
function InputBPM(int newBPM, int currentBPM){
	if(newBPM >= 300 OR newBPM <= 0){
		return currentBPM
	}
	return newBPM
}
```

The if statement is used to ensure the new value is within range. This is also used for inputting the top time signature number.

```
function InputTimeSignatureTopNum(int newTopNum, int currentTopNum){
	if(0 >= newTopNum OR newTopNum >= 21){
		return currentTopNum
	}
	return NewTopNum
}
```

```
function InputTimeSignatureBottomNum(int newBottomNum, int currentBottomNum){
	if(log(newTopNum,2) % 1 != 0 AND (newBottomNum > 16 OR newBottomNum < 1){
		return currentTopNum
	}
	return newTopNum
}
```

Since the bottom number can only be a power of two (identified in validation of inputs), the log base two is taken. It is then checked for a fractional part by then taking it modulo one, extracting only the fractional part. If there is a fractional part, then the new value cannot have been a power of two, as only powers of two return integers (numbers which lack a fractional part) when the log base two is taken. A range check is also performed.

```
function updateLightsSFXHaptics(int BPM, int topNum, int bottomNum, int activeLight, bool running){
	if(!running) return
	delay((60*BPM)/(bottomNum/4)
	vibrate()
	playSFX()
	return (activeLight+1)%topNum
}
```

An if statement is used such that this function only has effect if the metronome is running.
Then a delay is used (measured in seconds). A conversion has to be made from BPM to seconds. First beats per minute is converted to Minutes per Beats by taking the inverse of the current BPM. Next minutes are converted to seconds by a conversion factor of x60. This is then divided by a quarter of the bottom number (the subdivision). This can simplify to make the subdivision x240 and simply divide by just the subdivision. 

## Practice Tracker

As a database is planned to be used to store practice sessions, SQL commands to create, read, update, and delete were written. These SQL commands allowed for searching, updating and deleting by id and by date.

```sqlite
CREATE TABLE IF NOT EXISTS sessions (
	id   INTEGER PRIMARY KEY AUTOINCREMENT,
	date TEXT    NOT NULL,
	info TEXT    NOT NULL
)
```

```sqlite
INSERT INTO sessions (date, info)
VALUE(givenDate, givenInfo)
```

```sqlite
SELECT * FROM sessions
```

```sqlite
SELECT date, info FROM sessions
```

```sqlite
SELECT date, info FROM sessions
WHERE id LIKE targetId
```

```sqlite
SELECT date, info FROM sessions
WHERE date LIKE targetDate
```

```sqlite
UPDATE sessions
SET date = newDate
WHERE date LIKE targetDate
```

```sqlite
UPDATE sessions
SET   date = newDate
WHERE id   LIKE targetId
```

```sqlite
UPDATE sessions
SET   info = newInfo
WHERE date LIKE targetDate
```

```sqlite
UPDATE sessions
SET   info = newInfo
WHERE id   LIKE targetId
```

```sqlite
DELETE FROM sessions
WHERE id like targetId
```

```sqlite
DELETE FROM sessions
WHERE date like targetDate
```

