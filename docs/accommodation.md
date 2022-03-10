# Accommodation

An Accommodation typically represents a booked seat or berth (e.g. for a sleeper train).

For example, it knows which coach and seat number has been reserved for the passenger.

Belongs to an [OrderSeatReservation](/models/order-seat-reservation).

## Passengers vs Accommodations

There isn't always a direct one-to-one mapping of passengers to accommodations

- children under a certain age may travel for free and thus may not be registered as a passenger, so passengers < seats
- children (babies) may not require a seat (e.g. sit on parent's lap), so passengers > seats

## Deutsche Bahn

Note that Deutsche Bahn bookings will not have any accommodation records. The passenger will need to refer to their ticket to find out which coach and seat number they have been reserved.

```json jsonSchema
{
  "$ref": "./ordersDefinitions.oas2.yml#/definitions/accommodation"
}
```
