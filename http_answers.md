# HTTP Analysis (http://neverssl.com)

1. **Website Name:** neverssl.com

2. **First GET Request Packet:**
   The first GET request is:
   ```
   GET / HTTP/1.1
   ```

3. **Headers in GET Request:**
   - Host: neverssl.com
   - User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64)
   - Accept: text/html,application/xhtml+xml
   - Accept-Language: en-US,en;q=0.5
   - Connection: keep-alive

4. **Status Code in First Response:**
   `200 OK`

5. **Total HTTP Responses:**
   2 (HTML file + favicon)

6. **Persistent Connection:**
   Yes, because the `Connection: keep-alive` header was present, meaning multiple responses came over the same TCP connection.
