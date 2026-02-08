# Holiday Event Planner

Professional holiday event planner email template for inviting guests to a festive gathering within the hospitality and events industries.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Hospitality, Events
- **Message Type:** Events
- **Tags:** invitation, schedule, holidayparty, rsvp

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/holiday-event-planner.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/holiday-event-planner/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.holiday-event-planner',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
