# Updating Order Status

#### Nodes Summary:

- `wp_to_fb_order_id`
- `orders_statuses`



### `wp_to_fb_order_id`:

Use this node to get the Firebase `order_id`.

Give it the `order_id` from Wordpress.....and it will return the `id`of that order in Firebase.

`wp_to_fb_order_id` -> `wordpress_order_id` -> `firebase_order_id`



Now assume we have retreived the `firebase_order_id`.



### `orders_statuses`:

Set the status of that order in this node like so.

```javascript
"orders_statuses" : {
    "firebase_order_id" : "pending"
}
```



## Supported Statuses:

* pending
* confirmed
* cooking
* ready
* delivered
