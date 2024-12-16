
### Key Files and Directories

- **`app.py`**: The main application file that defines routes and handles requests.
- **`approaches/`**: Contains classes powering the Chat and Ask tabs.
- **`requirements.txt`**: Lists the Python dependencies required for the backend.

## Routes

### Chat Route

```python
@bp.route("/chat", methods=["POST"])
@authenticated
async def chat(auth_claims: Dict[str, Any]):
    #...