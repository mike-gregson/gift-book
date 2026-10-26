# Gift Lists

Shared language for managing gift lists, their recipients, and gifts among registered users.

## Language

**Gift List**:
A named collection of recipients and gifts managed by one owner and potentially shared with collaborators; it can have an optional occasion date.
_Avoid_: List

**Occasion Date**:
The date associated with a gift list's occasion, used to show a countdown until the date arrives. Passing the date does not archive the list.

**List Owner**:
The user accountable for a gift list, its membership and archive state, and its name, occasion date, and currency.
_Avoid_: Admin

**Collaborator**:
A user invited to edit a shared gift list's recipients and gifts.
_Avoid_: Member, shared user

**Registered User**:
A person with an account whose email address has been verified.

**List Invitation**:
An invitation sent to a user's email address to collaborate on a gift list; a person without an account can accept after registering and verifying that same address. Pending invitations expire after seven days, can be resent by the owner, and are revoked when the list is archived.

**Recipient**:
A person represented by a display name in one gift list, with no account or contact details required. Recipients are shared by default, duplicate names are allowed, and the same person on another list is a separate recipient. Removing a recipient leaves their gifts unassigned.

**Private Recipient**:
A recipient visible only to the user who created them, including their gifts and contribution to list statistics. Their records remain inaccessible while the creator lacks list access and become available again if they rejoin.

**Gift**:
An item with a required name and optional URL, planned or tracked for at most one recipient, with an optional assignment while planning. Removing a gift permanently deletes it.

**Gift Status**:
The gift's current state: Idea, Purchased, Arrived, Wrapped, or Given. Only the current status is retained.

**Gift Price**:
A gift's single monetary amount, expressed in its gift list's currency; it can be edited before or after purchase, and Purchased-or-later prices count toward spend. Idea-status prices represent planned value.

**List Currency**:
The single currency used for a gift list's prices, initially defaulted from the owner's locale; it can be changed until a gift price is first recorded.

**Spend**:
The per-list sum of known gift prices for gifts at Purchased, Arrived, Wrapped, or Given status; Idea-status value is planned value. Gifts without a price are excluded from monetary totals but included in gift counts. Unassigned gifts count toward list totals but not recipient comparisons. Graphs show current values by status and recipient, not historical trends.

**Recipient Privacy**:
A recipient's creator can switch them between shared and private; the setting also applies to their gifts and contribution to list statistics.

**Unassigned Gift**:
A gift on a list that is not currently associated with a recipient.

**Ownership Transfer**:
An explicit change of a gift list's owner; the former owner remains a collaborator unless removed.

**Permanent Deletion**:
The irreversible removal of a gift list and all its recipients and gifts by its owner after explicit confirmation; distinct from archiving.

**Archived Gift List**:
A manually archived, read-only gift list accessible to its existing collaborators and restorable by its owner. Archiving revokes pending invitations; an occasion date passing does not archive it automatically.