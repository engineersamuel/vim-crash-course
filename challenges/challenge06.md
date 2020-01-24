# Challenge 06 - Find and Replace

This challenge is designed to introduce you to find and replace within a single file.

#### Commands

* `V` (shift+v) will enter into visual line mode
* `:s/` is the syntax to start writing a regex find and replace

These commands may be helpful but are not strictly necessary:

* `v` will enter into visual character mode
* `ctrl+v` will enter into visual block mode
* `:nohl` will stop highlighting.
* `%` will jump to the matching `[](){}`

## Challenge

Here are the modifications to the text that will need to be reversed:
* All o's have been replaced with 0s
* All e's have been replaced with 3s
* All a's have been replaced with 4s
* All t's have been replaced with 7s

The goal here is to reverse all the modifications.

L0r3m ipsum dolor si7 am37, cons3c737ur adipiscing 3li7, s3d do 3iusmod 73mpor incididun7 u7 labor3 37 dolor3 magna aliqua. U7 3nim ad minim v3niam, quis nos7rud 3x3rci7a7ion ullamco laboris nisi u7 aliquip 3x 3a commodo cons3qua7. Duis au73 irur3 dolor in r3pr3h3nd3ri7 in volup7a73 v3li7 3ss3 cillum dolor3 3u fugia7 nulla paria7ur. Exc3p73ur sin7 occa3ca7 cupida7a7 non proid3n7, sun7 in culpa qui officia d3s3run7 molli7 anim id 3s7 laborum.

Hint:

* If you wanted to change 1s to 0s you could type the following while in normal mode: `:s/1/0/g`


Here is another modification you can try, something that I've done frequently when converting a React class to a function:

Input:

```
class Welcome extends React.Component<Props> {
    render() {
        return (
            <>
                <h1>Hello, {this.props.firstName} {this.props.lastName}</h1>
                <p>Your age is {this.props.age}</p>
            </>
        );
    }
}
```

Desired Output:

```
const Welcome (props: Props) => {
    return (
        <>
            <h1>Hello, {props.firstName} {props.lastName}</h1>
            <p>Your age is {props.age}</p>
        </>
    );
}
```