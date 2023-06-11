## README

## REQUIREMENTS
1. User can give ticket title and description
2. User can attach a file with ticket
3. User can create help Ticket
4. Admin can reply on help ticket
5. Admin can reject or resolve the ticket
6. When admin takes action on ticket. Acknolodge the User

## DATABASE SCHEME
1. TICKETS - 
    -   title(string) {required}
    -   description(text) {required}
    -   status(open{default} 
    -   resolved rejected) 
    -   attahcments(string) {nullable}
    -   user_id(int) {required - filled by laravel}
status_changed_by_id(int)
2. Replies - 
    -   body(text) {required}
    -   user_id(int) {required - filled by laravel}
    -   ticket_id(int) {required - filled by laravel}
