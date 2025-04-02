
## 📂 How to Create a “Contents” Tab in Your Sidebar

### ✅ Steps to Add a Custom Contents Tab

1. **Click the plus (+) icon** in the sidebar to create a new tiddler.

2. In the **title field**, name it `Contents` (or anything you want — this name will appear in the sidebar tab).

3. In the **tags field**, add:  
   ```
   $:/tags/SideBar
   ```

4. In the **body** of the tiddler, paste this code:
   ```html
   <div class="tc-table-of-contents">
   <<toc-selective-expandable 'Contents' sort[title]>>
   </div>
   ```

5. Scroll down to the **"Add a new field"** section:  
   - Field name: `list-before`  
   - Field value: `$:/core/ui/SideBar/Open`  
   Then click **Add**.

6. **Click the checkmark (✓)** in the top right to save the tiddler.

---

### 📌 How It Works

- The new sidebar tab will appear as `Contents`.  
- Any tiddler tagged with `Contents` will automatically appear in the list.  
- If those tiddlers have their own tags, they will be expandable sub-items.

---
