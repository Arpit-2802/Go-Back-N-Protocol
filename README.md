<h1>Go-Back-N ARQ</h1>
<p>In Go back N ARQ is the sliding window protocol where N is the sender's window size. In this protocol, the sender has to go back to N places from the last transmitted packet if any of the frame is lost or acknowledgment is not received.</p>
<p>If the acknowledgment of a frame is not received within an agreed-upon time period, then all the frames available in the current window will be retransmitted. Suppose we have sent frame no 5, but we didn't receive the acknowledgment of frame no 5, and the current window is holding three frames, then these three frames will be retransmitted.</p>
<p>The code implements two conditions:<br/> 1) The packet from the Senders window is lost.<br/>2) Acknowledegment is Lost.
</p>
