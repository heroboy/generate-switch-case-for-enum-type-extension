# README

A typescript language service plugin to generate switch case for enum type.

![screenshot](screenshot.gif)

## How to use

Ensure the case block of switch statement is empty. Place the cursor on `switch` then the 'Show fix' icon will display.

## Supported types

```typescript

enum EnumType1
{
	A=123,B,C
}

const enum EnumType2
{
	A=1,B="",C=false
}

type Union1 = 1|2|true|"abc";
type Union2 = 1|2|EnumType1|boolean;

```