# Snapshot report for `test/prefer-math-trunc.mjs`

The actual snapshot is saved in `prefer-math-trunc.mjs.snap`.

Generated by [AVA](https://avajs.dev).

## Invalid #1
      1 | const foo = 1.1 | 0;

> Error 1/1

    `␊
    > 1 | const foo = 1.1 | 0;␊
        |             ^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(1.1);␊
    `

## Invalid #2
      1 | const foo = 111 | 0;

> Error 1/1

    `␊
    > 1 | const foo = 111 | 0;␊
        |             ^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(111);␊
    `

## Invalid #3
      1 | const foo = (1 + 2 / 3.4) | 0;

> Error 1/1

    `␊
    > 1 | const foo = (1 + 2 / 3.4) | 0;␊
        |             ^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(1 + 2 / 3.4);␊
    `

## Invalid #4
      1 | const foo = bar((1.4 | 0) + 2);

> Error 1/1

    `␊
    > 1 | const foo = bar((1.4 | 0) + 2);␊
        |                  ^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = bar((Math.trunc(1.4)) + 2);␊
    `

## Invalid #5
      1 | const foo = (0, 1.4) | 0;

> Error 1/1

    `␊
    > 1 | const foo = (0, 1.4) | 0;␊
        |             ^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc((0, 1.4));␊
    `

## Invalid #6
      1 | function foo() {return.1 | 0;}

> Error 1/1

    `␊
    > 1 | function foo() {return.1 | 0;}␊
        |                       ^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | function foo() {return Math.trunc(.1);}␊
    `

## Invalid #7
      1 | const foo = 1.4 | 0.;

> Error 1/1

    `␊
    > 1 | const foo = 1.4 | 0.;␊
        |             ^^^^^^^^ Use \`Math.trunc\` instead of \`| 0.\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0.\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(1.4);␊
    `

## Invalid #8
      1 | const foo = 1.4 | .0;

> Error 1/1

    `␊
    > 1 | const foo = 1.4 | .0;␊
        |             ^^^^^^^^ Use \`Math.trunc\` instead of \`| .0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| .0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(1.4);␊
    `

## Invalid #9
      1 | const foo = 1.4 | 0.0000_0000_0000;

> Error 1/1

    `␊
    > 1 | const foo = 1.4 | 0.0000_0000_0000;␊
        |             ^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0.0000_0000_0000\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0.0000_0000_0000\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(1.4);␊
    `

## Invalid #10
      1 | const foo = 1.4 | 0b0;

> Error 1/1

    `␊
    > 1 | const foo = 1.4 | 0b0;␊
        |             ^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0b0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0b0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(1.4);␊
    `

## Invalid #11
      1 | const foo = 1.4 | 0x0000_0000_0000;

> Error 1/1

    `␊
    > 1 | const foo = 1.4 | 0x0000_0000_0000;␊
        |             ^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0x0000_0000_0000\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0x0000_0000_0000\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(1.4);␊
    `

## Invalid #12
      1 | const foo = 1.4 | 0o0;

> Error 1/1

    `␊
    > 1 | const foo = 1.4 | 0o0;␊
        |             ^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0o0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0o0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(1.4);␊
    `

## Invalid #13
      1 | const foo = 1.23 | 0 | 4;

> Error 1/1

    `␊
    > 1 | const foo = 1.23 | 0 | 4;␊
        |             ^^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(1.23) | 4;␊
    `

## Invalid #14
      1 | const foo = ~~3.9;

> Output

    `␊
      1 | const foo = Math.trunc(3.9);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~~3.9;␊
        |             ^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #15
      1 | const foo = ~~111;

> Output

    `␊
      1 | const foo = Math.trunc(111);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~~111;␊
        |             ^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #16
      1 | const foo = ~~(1 + 2 / 3.4);

> Output

    `␊
      1 | const foo = Math.trunc(1 + 2 / 3.4);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~~(1 + 2 / 3.4);␊
        |             ^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #17
      1 | const foo = ~~1 + 2 / 3.4;

> Output

    `␊
      1 | const foo = Math.trunc(1) + 2 / 3.4;␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~~1 + 2 / 3.4;␊
        |             ^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #18
      1 | const foo = ~~(0, 1.4);

> Output

    `␊
      1 | const foo = Math.trunc((0, 1.4));␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~~(0, 1.4);␊
        |             ^^^^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #19
      1 | const foo = ~~~10.01;

> Output

    `␊
      1 | const foo = ~Math.trunc(10.01);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~~~10.01;␊
        |              ^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #20
      1 | const foo = ~~(~10.01);

> Output

    `␊
      1 | const foo = ~Math.trunc(10.01);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~~(~10.01);␊
        |              ^^^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #21
      1 | const foo = ~(~~10.01);

> Output

    `␊
      1 | const foo = ~(Math.trunc(10.01));␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~(~~10.01);␊
        |               ^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #22
      1 | const foo = ~~-10.01;

> Output

    `␊
      1 | const foo = Math.trunc(-10.01);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~~-10.01;␊
        |             ^^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #23
      1 | const foo = ~~~~10.01;

> Output

    `␊
      1 | const foo = Math.trunc(Math.trunc(10.01));␊
    `

> Error 1/1

    `␊
    > 1 | const foo = ~~~~10.01;␊
        |               ^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #24
      1 | function foo() {return~~3.9;}

> Output

    `␊
      1 | function foo() {return Math.trunc(3.9);}␊
    `

> Error 1/1

    `␊
    > 1 | function foo() {return~~3.9;}␊
        |                       ^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #25
      1 | const foo = bar >> 0;

> Output

    `␊
      1 | const foo = Math.trunc(bar);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = bar >> 0;␊
        |             ^^^^^^^^ Use \`Math.trunc\` instead of \`>> 0\`.␊
    `

## Invalid #26
      1 | const foo = bar << 0;

> Output

    `␊
      1 | const foo = Math.trunc(bar);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = bar << 0;␊
        |             ^^^^^^^^ Use \`Math.trunc\` instead of \`<< 0\`.␊
    `

## Invalid #27
      1 | const foo = bar ^ 0;

> Output

    `␊
      1 | const foo = Math.trunc(bar);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = bar ^ 0;␊
        |             ^^^^^^^ Use \`Math.trunc\` instead of \`^ 0\`.␊
    `

## Invalid #28
      1 | function foo() {return.1 ^0;}

> Output

    `␊
      1 | function foo() {return Math.trunc(.1);}␊
    `

> Error 1/1

    `␊
    > 1 | function foo() {return.1 ^0;}␊
        |                       ^^^^^ Use \`Math.trunc\` instead of \`^ 0\`.␊
    `

## Invalid #29
      1 | const foo = {a: {b: {c: 3}}};
      2 | const bar = a.b.c | 0;

> Error 1/1

    `␊
      1 | const foo = {a: {b: {c: 3}}};␊
    > 2 | const bar = a.b.c | 0;␊
        |             ^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = {a: {b: {c: 3}}};␊
      2 | const bar = Math.trunc(a.b.c);␊
    `

## Invalid #30
      1 | const foo = {a: {b: {c: 3}}};
      2 | const bar = a.b?.c | 0;

> Error 1/1

    `␊
      1 | const foo = {a: {b: {c: 3}}};␊
    > 2 | const bar = a.b?.c | 0;␊
        |             ^^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = {a: {b: {c: 3}}};␊
      2 | const bar = Math.trunc(a.b?.c);␊
    `

## Invalid #31
      1 | const foo = {a: {b: {c: 3}}};
      2 | const bar = ~~a.b?.c;

> Output

    `␊
      1 | const foo = {a: {b: {c: 3}}};␊
      2 | const bar = Math.trunc(a.b?.c);␊
    `

> Error 1/1

    `␊
      1 | const foo = {a: {b: {c: 3}}};␊
    > 2 | const bar = ~~a.b?.c;␊
        |             ^^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #32
      1 | const foo = 3;
      2 | const bar = foo | 0;

> Error 1/1

    `␊
      1 | const foo = 3;␊
    > 2 | const bar = foo | 0;␊
        |             ^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = 3;␊
      2 | const bar = Math.trunc(foo);␊
    `

## Invalid #33
      1 | const foo = 3;
      2 | const bar = ~~foo;

> Output

    `␊
      1 | const foo = 3;␊
      2 | const bar = Math.trunc(foo);␊
    `

> Error 1/1

    `␊
      1 | const foo = 3;␊
    > 2 | const bar = ~~foo;␊
        |             ^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #34
      1 | let foo = 2;
      2 | foo |= 0;

> Output

    `␊
      1 | let foo = 2;␊
      2 | foo = Math.trunc(foo);␊
    `

> Error 1/1

    `␊
      1 | let foo = 2;␊
    > 2 | foo |= 0;␊
        | ^^^^^^^^ Use \`Math.trunc\` instead of \`|= 0\`.␊
    `

## Invalid #35
      1 | const foo = {a: {b: 3.4}};
      2 | foo.a.b |= 0;

> Output

    `␊
      1 | const foo = {a: {b: 3.4}};␊
      2 | foo.a.b = Math.trunc(foo.a.b);␊
    `

> Error 1/1

    `␊
      1 | const foo = {a: {b: 3.4}};␊
    > 2 | foo.a.b |= 0;␊
        | ^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`|= 0\`.␊
    `

## Invalid #36
      1 | const foo = 10.01;
      2 | const bar = ~~foo;

> Output

    `␊
      1 | const foo = 10.01;␊
      2 | const bar = Math.trunc(foo);␊
    `

> Error 1/1

    `␊
      1 | const foo = 10.01;␊
    > 2 | const bar = ~~foo;␊
        |             ^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #37
      1 | let foo = 10.01;
      2 | foo >>= 0;

> Output

    `␊
      1 | let foo = 10.01;␊
      2 | foo = Math.trunc(foo);␊
    `

> Error 1/1

    `␊
      1 | let foo = 10.01;␊
    > 2 | foo >>= 0;␊
        | ^^^^^^^^^ Use \`Math.trunc\` instead of \`>>= 0\`.␊
    `

## Invalid #38
      1 | let foo = 10.01;
      2 | foo <<= 0;

> Output

    `␊
      1 | let foo = 10.01;␊
      2 | foo = Math.trunc(foo);␊
    `

> Error 1/1

    `␊
      1 | let foo = 10.01;␊
    > 2 | foo <<= 0;␊
        | ^^^^^^^^^ Use \`Math.trunc\` instead of \`<<= 0\`.␊
    `

## Invalid #39
      1 | let foo = 10.01;
      2 | foo ^= 0;

> Output

    `␊
      1 | let foo = 10.01;␊
      2 | foo = Math.trunc(foo);␊
    `

> Error 1/1

    `␊
      1 | let foo = 10.01;␊
    > 2 | foo ^= 0;␊
        | ^^^^^^^^ Use \`Math.trunc\` instead of \`^= 0\`.␊
    `

## Invalid #40
      1 | function foo() {return[foo][0] ^= 0;};

> Output

    `␊
      1 | function foo() {return[foo][0] = Math.trunc([foo][0]);};␊
    `

> Error 1/1

    `␊
    > 1 | function foo() {return[foo][0] ^= 0;};␊
        |                       ^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`^= 0\`.␊
    `

## Invalid #41
      1 | const foo = /* first comment */ 3.4 | 0; // A B C

> Error 1/1

    `␊
    > 1 | const foo = /* first comment */ 3.4 | 0; // A B C␊
        |                                 ^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = /* first comment */ Math.trunc(3.4); // A B C␊
    `

## Invalid #42
      1 | const foo = /* first comment */ ~~3.4; // A B C

> Output

    `␊
      1 | const foo = /* first comment */ Math.trunc(3.4); // A B C␊
    `

> Error 1/1

    `␊
    > 1 | const foo = /* first comment */ ~~3.4; // A B C␊
        |                                 ^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #43
      1 | const foo = {a: {b: 3.4}};
      2 | foo /* Comment 1 */ .a /* Comment 2 */ . /* Comment 3 */ b |= /* Comment 4 */ 0 /* Comment 5 */;

> Output

    `␊
      1 | const foo = {a: {b: 3.4}};␊
      2 | foo /* Comment 1 */ .a /* Comment 2 */ . /* Comment 3 */ b = Math.trunc(foo /* Comment 1 */ .a /* Comment 2 */ . /* Comment 3 */ b) /* Comment 5 */;␊
    `

> Error 1/1

    `␊
      1 | const foo = {a: {b: 3.4}};␊
    > 2 | foo /* Comment 1 */ .a /* Comment 2 */ . /* Comment 3 */ b |= /* Comment 4 */ 0 /* Comment 5 */;␊
        | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`|= 0\`.␊
    `

## Invalid #44
      1 | const foo = {a: {b: 3.4}};
      2 | const bar = /* Comment 1 */ ~~ a /* Comment 3 */ . /* Comment 4 */ b /* Comment 5 */;

> Output

    `␊
      1 | const foo = {a: {b: 3.4}};␊
      2 | const bar = /* Comment 1 */ Math.trunc(a /* Comment 3 */ . /* Comment 4 */ b) /* Comment 5 */;␊
    `

> Error 1/1

    `␊
      1 | const foo = {a: {b: 3.4}};␊
    > 2 | const bar = /* Comment 1 */ ~~ a /* Comment 3 */ . /* Comment 4 */ b /* Comment 5 */;␊
        |                             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #45
      1 | const foo = /* will keep */ 3.4 /* will remove 1 */ | /* will remove 2 */ 0;

> Error 1/1

    `␊
    > 1 | const foo = /* will keep */ 3.4 /* will remove 1 */ | /* will remove 2 */ 0;␊
        |                             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = /* will keep */ Math.trunc(3.4);␊
    `

## Invalid #46
      1 | const foo = /* will keep */ ~ /* will remove 1 */ ~ /* will remove 2 */ 3.4;

> Output

    `␊
      1 | const foo = /* will keep */ Math.trunc(3.4);␊
    `

> Error 1/1

    `␊
    > 1 | const foo = /* will keep */ ~ /* will remove 1 */ ~ /* will remove 2 */ 3.4;␊
        |                             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #47
      1 | const foo = 3.4; // comment 1
      2 | foo |= 0; // comment 2

> Output

    `␊
      1 | const foo = 3.4; // comment 1␊
      2 | foo = Math.trunc(foo); // comment 2␊
    `

> Error 1/1

    `␊
      1 | const foo = 3.4; // comment 1␊
    > 2 | foo |= 0; // comment 2␊
        | ^^^^^^^^ Use \`Math.trunc\` instead of \`|= 0\`.␊
    `

## Invalid #48
      1 | const foo = 3.4; // comment 1
      2 | const bar = ~~foo; // comment 2

> Output

    `␊
      1 | const foo = 3.4; // comment 1␊
      2 | const bar = Math.trunc(foo); // comment 2␊
    `

> Error 1/1

    `␊
      1 | const foo = 3.4; // comment 1␊
    > 2 | const bar = ~~foo; // comment 2␊
        |             ^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #49
      1 | const foo = ~~bar | 0;

> Output

    `␊
      1 | const foo = Math.trunc(bar) | 0;␊
    `

> Error 1/2

    `␊
    > 1 | const foo = ~~bar | 0;␊
        |             ^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(~~bar);␊
    `

> Error 2/2

    `␊
    > 1 | const foo = ~~bar | 0;␊
        |             ^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

## Invalid #50
      1 | const foo = ~~(bar| 0);

> Output

    `␊
      1 | const foo = Math.trunc(bar| 0);␊
    `

> Error 1/2

    `␊
    > 1 | const foo = ~~(bar| 0);␊
        |             ^^^^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

> Error 2/2

    `␊
    > 1 | const foo = ~~(bar| 0);␊
        |                ^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = ~~(Math.trunc(bar));␊
    `

## Invalid #51
      1 | const foo = bar | 0 | 0;

> Error 1/2

    `␊
    > 1 | const foo = bar | 0 | 0;␊
        |             ^^^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(bar | 0);␊
    `

> Error 2/2

    `␊
    > 1 | const foo = bar | 0 | 0;␊
        |             ^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = Math.trunc(bar) | 0;␊
    `

## Invalid #52
      1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);

> Output

    `␊
      1 | const foo = Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(bar | 0 | 0))))))));␊
    `

> Error 1/9

    `␊
    > 1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`~~\`.␊
    `

> Error 2/9

    `␊
    > 1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`^ 0\`.␊
    `

> Error 3/9

    `␊
    > 1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`^ 0\`.␊
    `

> Error 4/9

    `␊
    > 1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`<< 0\`.␊
    `

> Error 5/9

    `␊
    > 1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`<< 0\`.␊
    `

> Error 6/9

    `␊
    > 1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`>> 0\`.␊
    `

> Error 7/9

    `␊
    > 1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`>> 0\`.␊
    `

> Error 8/9

    `␊
    > 1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                   ^^^^^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = ~~~~((Math.trunc(bar | 0)) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
    `

> Error 9/9

    `␊
    > 1 | const foo = ~~~~((bar | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                   ^^^^^^^ Use \`Math.trunc\` instead of \`| 0\`.␊
    ␊
    --------------------------------------------------------------------------------␊
    Suggestion 1/1: Replace \`| 0\` with \`Math.trunc\`.␊
      1 | const foo = ~~~~((Math.trunc(bar) | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
    `

## Invalid #53
      1 | const foo = Array.from({length: 10}, (_, index) => (index + 1) + (index + 1) /100);
      2 | let i = 0;
      3 | while (i < foo.length) {
      4 | 	foo[i++] |= 0;
      5 | }
      6 | console.log(foo);

> Error 1/1

    `␊
      1 | const foo = Array.from({length: 10}, (_, index) => (index + 1) + (index + 1) /100);␊
      2 | let i = 0;␊
      3 | while (i < foo.length) {␊
    > 4 | 	foo[i++] |= 0;␊
        | 	^^^^^^^^^^^^^ Use \`Math.trunc\` instead of \`|= 0\`.␊
      5 | }␊
      6 | console.log(foo);␊
    `
