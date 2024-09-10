# poorly-made-notes

```c
extern const char* NOT_REALLY_SURE_IF_THIS_EXISTS; // beg for someone implement this in linker scripts
static const volatile char** POORLY_MADE_NOTES = &NOT_REALLY_SURE_IF_THIS_EXISTS;

extern puts(const char* str); // hoping you implement this with proper serial port

void entry_point(){
	puts("Welcome to this poorly made notes\n"
		 "Except for linear system, which are made to be able read"
		 "online on github. The rest are not meant to be render"
		 "properly on github. Therefore its better to just load"
		 "these into obsidian for better readability"
	);
}
```