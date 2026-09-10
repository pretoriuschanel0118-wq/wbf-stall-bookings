WEES BEES FEES 2026 – INTERACTIVE STALL BOOKING

Files:
- index.html: complete vendor/admin website
- slide2.png: source PowerPoint Slide 2 map
- slide3.png: source PowerPoint Slide 3 FM map
- slide4.png: source PowerPoint Slide 4 key

Database:
The HTML is written for the current Supabase schema:
- stalls.blocked_permanently (NOT stalls.active or stalls.is_blocked)
- bookings.stall_id, bookings.size, bookings.business, bookings.contact, bookings.phone, bookings.email, bookings.sell, bookings.booked_at
- RPC confirm_stall(p_stall_id, p_size)
- RPC admin_block_stall(p_stall_id)
- RPC admin_unblock_stall(p_stall_id)
- RPC admin_release_booking(p_booking_id)

Important:
The website no longer queries stalls.active. This removes the "column stalls.active does not exist" error.
